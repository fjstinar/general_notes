This contains temporary code for the [[RETTL Web Extension]] Debugging

### background.js
To download data from the server
```
const downloadDataFromFixedUrl = async () => {
  const url = 'https://mcdataservice.humanplusml.com/download';
  const filename = `data_${new Date().toISOString()}`;

  try {
    const response = await fetch(url, {
      method: 'GET',
      headers: {
        'Content-Type': 'application/json'
      }
    });

    if (response.ok) {
      const contentType = response.headers.get('Content-Type');

      let dataStr;
      let fileExtension;

      if (contentType.includes('application/json')) {
        // If the response is JSON
        const data = await response.json();
        dataStr = JSON.stringify(data, null, 2);
        fileExtension = 'json';
      } else if (contentType.includes('text')) {
        // If the response is plain text or HTML
        dataStr = await response.text();
        fileExtension = 'txt';
      } else {
        // Handle other content types (e.g., binary data)
        const blob = await response.blob();
        const downloadUrl = URL.createObjectURL(blob);

        const downloadLink = document.createElement('a');
        downloadLink.href = downloadUrl;
        downloadLink.download = `${filename}.bin`;

        // Simulate a click on the download link
        downloadLink.click();

        // Clean up the URL object
        URL.revokeObjectURL(downloadUrl);

        console.log('Binary data downloaded successfully');
        return;
      }

      const blob = new Blob([dataStr], { type: contentType });
      const downloadUrl = URL.createObjectURL(blob);

      const downloadLink = document.createElement('a');
      downloadLink.href = downloadUrl;
      downloadLink.download = `${filename}.${fileExtension}`;

      // Simulate a click on the download link
      downloadLink.click();

      // Clean up the URL object
      URL.revokeObjectURL(downloadUrl);

      console.log('Data downloaded successfully');
    } else {
      console.error('Failed to fetch data. HTTP Status:', response.status);
    }
  } catch (error) {
    console.error('Fetch error:', error.message);
  }
};

(chrome || browser).runtime.onMessage.addListener((message, sender, sendResponse) => {
  if (message.type === 'downloadData') {
    downloadDataFromFixedUrl();
    sendResponse({ status: 'Data download initiated' });
  }

  return true;
});

```

### popup.js
To download data from the server
```
document.getElementById('download-data').addEventListener('click', () => {

chrome.runtime.sendMessage({ type: 'downloadData' }, (response) => {

console.log(response.status);

});

});
```
