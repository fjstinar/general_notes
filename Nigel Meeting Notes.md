#### 11.4.2024 (Actually Ruohan Meeting)
60 control 70 experiment
For specific reviewer comments - maybe use one-tailed instead of two-tailed
Could we do a two-tailed for overall and one-tailed for the subthings

+75 ~$1500
+135

#### 11.2.2024
- Singular method
- use gender instead of sex
- Number letter instead for the list of things under method section
- Blow up the text in the pipeline figure
- Line drawn with labels for the first pie chart

Results part 1: unequal base rate could make the problem difficult
Results point 2. Add ',' after consistently
Metrics are incongruent with improving accuracy on point 4
 - Add Kappa and AUC measures for accuracy
 
- Text bigger on graphs and text bigger on the figures
- move labels inside of pie chart
- '+' and '-' over positive and negative
- 'High' and 'Low'
- (High vs Low grade) with high and low description'

Synthetic data - simulate.
Change to a Portuguese course. rather than Portuguese language subject.

Change title of figures to black


#### 10/30/2024
- Could shift to showing an overall model is biased, then break it down and see how that shifts with different data sources integrated

- fair feature selection. Apply this method. Unfairness metrics.py. Sequential feature selector with the ffs github combined metric is the whole point of that method
	- the order of the features can't be found but. can run sequential feature selection.
	- crank the unfairness parameter the way up and compare it to accuracy. Do it on a scale of 0 to 2. Use this method to determine what features are the fair features...
- L@S
- 5 Papers



Resubmission of CHI one reframing/spell checking -> not too difficult L@S or EDM
LAK -> Resubmission AIED or EDM...
A lot of writing for Hanning paper -> EDM
Positionality survey a lot of writing -> EDM



#### 10/22/24

Collect more information from experiment parts

------
Calculate chronbach's alpha of the scales. if it is high then it is just correct

Careful wording on how the three factors are different
women could have more of an appreciation for methods that account for marginalization
- could be a possiblity
Potentially students from more minoritized group are more accepting of additional information

women students dont agree that an increased accuraacy justifies using increased

- py-description checks if student is under/overconfident and takes them to different study components - do this ASAP
- might have to modify the pretest to act more like the navigation component
- could set the 'next-component-id' to using the javascript
- 'this.next_component_id'
	- not quite a survey component
- different completion code for the screened-out participants


non parametric anova for the factor loadings. non parametric correlation for the other two.

Scales for idealism and relativism...

correlate with the factors with relativism and idealism...

make sure we follow the specific tests from the preregistration

female participants are more into academics and less into political affiliation

EDM, AIED, UMAP, L@S, FACCT
notes

spend time thinking about more participants


-correlation matrix between the variables

-spearman correlations for idealism/relativism/gender/political affiliation. one hot encode race for extra columns in the correlation matrix

-confidence interval to say approximately how big the effect could be....... Moving forward



#### 10/08/24
RETTL
	- slope of regression as scaling factor
	- $274.07 $1.85 per person
		- for underconfident 100 people for two variations. $1500 for underconfident participants
	- get some browser plugin updates

#### 10/04/24
RETTL
	- email Karle for access to mastery/what webpages are used for STAT 107
	- capture when youtube videos were watched/make sure it doesnt track ALL youtube videos (only on the tracked URL)
	- power analysis/estimate the time it took to complete the pretest
AI Positionality Survey
	- post hoc test for what is teh difference (non-parametric t-test wilcoxin test)
	- Check if AI_added are correlated with eachother
	- Other updates from notes on remarkable

#### 10/01/24
RETTL
	- look at vidprobe repo updates for underconfident learners


#### 09/23/24
RETTL
	- Data collection is now happening in STAT 107
	- Also uses mastery.cs.illinois.edu
	- For unfairness mitigation needs shap values before/after unfairness mitigation step
	- Attention RF could rely to much on the feature so I should check the hyperparameters of both models
	- Furthermore, could bootstrap for significant differences between the datasets
	- Could combine with HaeJin's dataset
AI Positionality Survey
	- Calculate difference for all questions individually
		- Non parametric ANOVA
		- Kruskal-wallis Test then find differences'
		- Use odd graph style Nigel drew
		- Calulate the actual loadings of the factors