Notion: https://www.notion.so/Fairness-everywhere-c851506c41bd432d91120f6372c87caf?pvs=4


Choose datasets that contain the biases represented within education



| Title                                                                                                                | Conference | Year | Algorithm                                                 | Bias Measurement                      | Applied Bias Mitigation                       | isFairness? |
| -------------------------------------------------------------------------------------------------------------------- | ---------- | ---- | --------------------------------------------------------- | ------------------------------------- | --------------------------------------------- | ----------- |
| A Data Mining Approach for Detecting Collusion in Unproctored Online Exams                                           | EDM        | 2023 | Hierarchical Clustering                                   | None                                  | None                                          | No          |
| Analysis of an Explainable Student Performance Prediction Model in an Introductory Programming Course                | EDM        | 2023 | Explainable stacked ensemble model                        | None                                  | None                                          | No          |
| Is Your Model "MADD"? A Novel Metric to Evaluate Algorithmic Fairness for Predictive Student Models                  | EDM        | 2023 | Logistic regression, KNN, decision tree, naive bayes      | MADD metric                           | None                                          | Yes         |
| Investigating the Importance of Demographic Features for EDM-Predictions                                             | EDM        | 2023 | Generalized Linear Models, XGBoost                        | None                                  | None                                          | Yes         |
| Scalable and Equitable Math Problem Solving Strategy Prediction in Big Educational Data                              | EDM        | 2023 | Clustering Embeddings into a LSTM                         | Disparate Mistreatment                | None                                          | Yes         |
| Generalizing Predictive Models of Reading Ability in Adaptive Mathematics Software                                   | EDM        | 2023 | Multi-layer perceptron                                    | Performance on different demographics | None                                          | Yes         |
| Partner Keystrokes can Predict Attentional States during Chat-based Conversations                                    | EDM        | 2023 | lme4 mixed-effects models                                 | None                                  | None                                          | No          |
| The Predictiveness of PFA is Improved by Incorporating the Learner's Correct Response Time Fluctuation               | EDM        | 2023 | PFA, Logistic Knowledge Tracing                           | None                                  | None                                          | No          |
| Towards Generalizable Detection of Urgency of Discussion Forum Posts                                                 | EDM        | 2023 | Random forest. XGB, LR, Ordinal Ridge Regression, SVR, NN | None                                  | None                                          | No          |
| Early Prediction of Student Performance in a Health Data Science MOOC                                                | EDM        | 2023 | Markov chain into NN                                      | None                                  | None                                          | No          |
| Towards Scalable Adaptive Learning with Graph Neural Networks and Reinforcement Learning                             | EDM        | 2023 | Graph NN/Reinforcement Learning                           | None                                  | None                                          | No          |
| Auto-scoring Student Responses with Images in Mathematics                                                            | EDM        | 2023 | OCR + CNN, SBERT-Canberra Model                           | None                                  | None                                          | No          |
| Modeling and Analyzing Scorer Preferences in Short-Answer Math Questions                                             | EDM        | 2023 | BERT                                                      | None                                  | None                                          | No          |
| Predicting Bug Fix Time in Students' Programming with Deep Language Models                                           | EDM        | 2023 | transformer + LSTM                                        | None                                  | None                                          | No          |
| Predicting GRE Scores from Application Materials in Test-Optional Admissions                                         | EDM        | 2024 | Tree, RF, LR, NN, XGBoost                                 | Difference in predictions             | None                                          | No          |
| Says Who? How different ground truth measures of emotion impact student affective modeling                           | EDM        | 2024 | Affect detectors                                          | None                                  | None                                          | No          |
| Multimodal Learning Analytics for Predicting Student Collaboration Satisfaction in Collaborative Game-Based Learning | EDM        | 2024 | LSTM, RNN                                                 | None                                  | None                                          | No          |
| Examining the Algorithmic Fairness in Predicting High School Dropouts                                                | EDM        | 2024 | LR, SVM, XGB, NN, RF                                      | Differential algorithmic functioning  | None                                          | Yes         |
| Early Prediction of Student Dropout in Higher Education using Machine Learning Models                                | EDM        | 2024 | NN, XGBoost                                               | None                                  | None                                          | No          |
| Investigation of behavioral Differences: Uncovering Behavioral Sources of Demographic Bias in Educational Algorithms | EDM        | 2024 | jade                                                      | jade                                  | jade                                          | jade        |
| Plagiarism Detection Using Keystroke Logs                                                                            | EDM        | 2024 | LDA, MLP, RF, SVM                                         | None                                  | None                                          | No          |
| From Reaction to Anticipation: Predicting Future Affect                                                              | EDM        | 2024 | Affect detectors                                          | None                                  | None                                          | No          |
| Fair Prediction of Students' Summative Performance Changes Using Online Learning Behavior Data                       | EDM        | 2024 | LR, SVM, DT, RF, KNN, NN                                  | treatment equality                    | treatment equality constraint during training | Yes         |
|                                                                                                                      |            |      |                                                           |                                       |                                               |             |






10/18/2024
focus on where the biases come from



10/14/2024 Kick off
Number of key educational contexts where things are being used
then look at contexts in the biases.

could have missing data problems in some datasets versus other datasets

redo tagging system based on previous work

group datasets based on the previous bias. Frame datasets

- recent surveys and how we chose methods
- then strategy for picking datasets using bias types used in some other survey paper
- then introduce that we care about other things for real world stakeholders
	- define each category in one or two paragraphs

complexity of the model. Simpler method

contribution of real way to apply the methods using the techniques

types of bias we expect in the datasets. (e.g., bad on representation/ some framework on bias types/)

problem is which of these techniques are feasible to employ/practical in the context.

selected datasets in the landscape that are representative of the problems in the data

build bridges between the two...

Add in tags that position it for learning scientists. And in education

dont have to defend the tagging system if another review did it. Look into how these big reviews tagged papers

Report averages for six datasets

**Dataset Coverage**
*Preference towards larger, structured datasets, highest priority dimensions (type of data, type of task)*

*Demographics* - sexual orientation, field, year of schooling, age, ethnicity, race, country of education, sex, gender, language schooling, socio economic background, behavior, ELL, Caste, disability, highest education, diploma

*Type of Data* - Q&A, videos, clickstream, demographics, grades, behavior

*Type of Task* - Drop out prediction, on-time graduation, intervention prediction, grade prediction, mastery, gaming prediction

We also want possible diverse contexts and sizes

Maybe could use Combinatorial Coverage

Minimum Items Needed $= max(Size, Type of Task) = max(5, 6) = 6$


**Only open source**

| Dataset                       | Size   | Demographic                                                  | Type of Data                                | Type of Task                          | Context         | Where         |
| ----------------------------- | ------ | ------------------------------------------------------------ | ------------------------------------------- | ------------------------------------- | --------------- | ------------- |
| OULAD                         | $10^4$ | SES, Sex, Gender, Age, Disability, Highest Ed, Country of Ed | Behavior, Demographics, Clickstream, Grades | Grade Prediction                      | MOOC            | EU            |
| Math and Portuguese           | $10^2$ | Year of schooling, Age, SES, Sex                             | Demographics, Grades                        | Grade Prediction                      | Highschool      | EU?           |
| XuetangX                      | $10^3$ | Gender, Diploma, Age                                         | Demographics, Grades                        | Drop Out Prediction                   | University MOOC | Asia          |
| EEDI                          | $10^5$ | Age, Gender, SES                                             | Demographics, Behavior                      | Mastery                               |                 | EU            |
| Student Academics Performance | $10^2$ | Gender, SES, Caste                                           | Demographics, Grades, Behavior              | Grade Prediction, Drop Out Prediction | University      | Asia          |
| From Here To There            | $10^4$ | Gender, Ethnicity                                            | Demographics, Clickstream                   | Mastery, Grade Prediction             | Middle School   | North America |

Possible updates:

Nigel could be involved. Tanja 

To-do:
Tag datasets and methods and make statistic of what type of method is use don what type of dataset

Inprocessing, preprocessing, \

FAACT, educational conferences, NEURIPS

https://dl.acm.org/doi/10.1145/3531146.3533113

[![](https://dl.acm.org/pb-assets/head-metadata/apple-touch-icon-1574252172393.png)ACM Other conferencesAn Algorithmic Framework for Bias Bounties | Proceedings of …](https://doi.org/10.1145/3531146.3533172)​

**October 5th Jade Birthday**


Question about fairness inprocessing and normal inprocessing with the tagging system

Tuesday Bring up with Nigel with the supervision/meeting things?