Overleaf: https://www.overleaf.com/project/667207a92015bec699c48eba

Paper Additions:
- [x] Explain specific numbers in intervention groups
- [x] Add demographic groups/base rates (Give specific responses)
- [ ] 2.2 add existing studies that improve MCC
- [ ] Possibly integrate HCI theories
- [x] Describe ML prediction model

### Machine Learning Model Description
Alongside providing the interventions, our online learning platform also modeled student learning gain by predicting their score on the posttest that is given at the end of the learning session. The model is trained on interaction data from **X** students in a previous study using the same online learning platform. Specifically, the model is trained two types of data: performance data and interaction data. The performance data consisted of the pretest score and quiz scores of each of the four topics in the learning session. The interaction data records the time spent on certain facets of the learning session and the counts of accesses to different types of content. Specifically, we trained a **random forest model with attention** to predict the posttest score of each student in the experiment condition throughout their learning session. 

Alongside the metacognitive calibration interventions, every 15 minutes the current machine learning model prediction is shown to the students. The prediction is presented on a separate page after the intervention is completed. We describe to the students that the model made this prediction based on the students' own interactions with the platform, and we offer a few general ways the student can improve their prediction.

