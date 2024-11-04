Overleaf: https://www.overleaf.com/project/667207e1e577ab9fc72a0bc1

SEPTEMBER 5th ABSTRACT DUE

Papers to find:
- [ ] Neil Heffernan EDM a few years ago. RCT with assistments data
- [ ] LAK 2023 Fanscali Emerging Readers definitions
	- [ ] to help show that it is a feature that is being used in the real world

To-Do Analyses:
- [x] Bootstrap to compare the current findings. Use this to conduct statistical tests
	- [x] Draw many bootstrap samples to check if they are different
	- [x] bootstrap all differences to test for statistical significance. namely the base rates (control - emerging) [[Significance Tests]]
		- [x] Mean difference between predictions (Pred - True) \[0.0368, 0.0504\]
		- [ ] 
- [x] Find absolute value of the metrics
- [x] calculate avg prediction PER student
- [x] Lump year 11 with year 12
- [x] Calculate bootstrap metrics with the unfairness mitigated datasets

For Paper:
- [x] Refer to Husni model as an estimator or a measurement method. by measuring ELL status in terms of MATHia interactions, we are capturing the characteristics that are manifested in MATHia. ELL Labels are specifically meaningful for the interaction patterns.
- [x] Implication of possible threshold adjustment for mastery
- [ ] We chose RMSE because we do believe that large outliers should be penalized more
- [x] Could include size of dataset in the abstract
- [x] (difference p<.001)
- [x] make sure I define workspaces. In abstract change workspaces to math topics
- [x] difference in means stat symbol
- [x] include difference in means alongisde confidence intervals
- [ ] include statistical parity in abstract
- [x] conceptulaly say that our findings imply that reading ability is an essential consideration in the design of equitable math education software
- [x] jump straight into emerging readers problem. e.g., student reading ability affects their interactions even in learning software in unrelated domains which can result in inequitable outcomes
- [ ] describe the units of confidence intervals
- [x] move captions of table to the tops
- [x] confidence intervals should have square brackets
- [x] two subsections in the table. The first being the first three columns (overall) the second being the comparisons between groups
- [ ] add in caption the mean diffference in auc between reweighing and not reweighing
- [ ] add spaces between words and parentheses
- [ ] best/worst/median. state that we are choosing those in particular
- [x] confidence interval graph
- [x] add calibration bootstrapping method
- [x] color bars right next to each other for means
- [x] also graph difference in calibration
- [x] remove the first three confidence interval things
- [x] first table is graph for the four things
- [ ] look at Clara LAK draft


About trying to explain to one of my friends in college... If he cant understand then nobody understands. Add additions to explain things......

Export as PDF. Put reweighing in the caption. Value of 0 indicates no difference between means (y-axis nonemerging - emerging).

Despite datase size and focusing on the most popular workspaces there are still issues related to workspace specific sample size to make it not possible for workspace specific reweighing


Figure 1: Plot of point estimates and confidence intervals for differences between means of emerging and non-emerging readers, with estimates grouped by dataset (academic year) and reweighing versus no reweighing. The data show that reweighing makes little difference in fairness, with perhaps very slight improvement (i.e., less difference between groups) in terms of RMSE and predicted rates. Base rates most notably differ between groups (approximately .08) while predictions differ somewhat (approximately .04) and RMSE and calibration differ little between groups.

Table 1: Table of measurements for the aggregate BKT model predictions. The two original datasets and the datasets after being preprocessed with reweighing are evaluated on AUC, RMSE, statistical parity, disparate impact, and average odds. The data show that reweighing makes little difference in AUC, RMSE, and fairness.  Furthermore, both of the original datasets have some bias against emerging readers based on the fairness metrics.

Table 2: Table of measurements for skill-focused BKT models. Three skills are displayed with their reweighed counterparts and are evaluted on AUC, RMSE, statistical parity, disparate impact, and average odds. The reweighing method had minimal impact on the evaluations. There is varying levels of AUC (.512 to .771), RMSE (.285 to .439), statistical parity (-.263 to -.009), disparate impact (.609 to .991), and average odds (-.181 to -.007) across the BKT models for the three different skills.



University ethics review boards have approved the human-subject research and have approved this project. Also, all data has been properly anonymized by the MathITS team.