Brockton 21-22

	Overall RMSE (True - Pred): (0.0646, 0.0682)   |RW: (0.0645, 0.0680)
	RMSE (True - Pred) NonEmerge: (0.0638, 0.0675) |RW: (0.0638, 0.0674)
	RMSE (True - Pred) Emerging: (0.0642, 0.0736)  |RW: (0.0640, 0.0731)

| Comparison (NonEmerge - Emerging) | CI (95%)          | Reweighing        | Non      | Emerge | Non (RW)    | Emerge (RW) |
| --------------------------------- | ----------------- | ----------------- | -------- | ------ | ----------- | ----------- |
| Mean predictions                  | (0.0366, 0.0503)  | (0.0367, 0.0504)  | .7514172 |        | 0.04348629  |             |
| Mean True Values                  | (0.0747, 0.0950)  | (0.0748, 0.0949)  | .77501   |        | 0.08492827  |             |
| Mean RMSE (True - Pred)           | (-0.0079, 0.0018) | (-0.0081, 0.0021) | -0.0029  |        | -0.00280857 |             |
| Calibration                       | (0.0007, 0.0084)  | (0.0009, 0.0086)  | .0046    |        | 0.004812934 |             |


Brockton 22-23

	Overall RMSE (True - Pred): (0.0676, 0.0724)   |RW: (0.0677, 0.0726)
	RMSE (True - Pred) NonEmerge: (0.0674, 0.0725) |RW: (0.0675, 0.0727)
	RMSE (True - Pred) Emerging: (0.0646, 0.0761)  |RW: (0.0646, 0.0764)

| Comparison (NonEmerge - Emerging) | CI (95%)          | Reweighing        |               | rw           |
| --------------------------------- | ----------------- | ----------------- | ------------- | ------------ |
| Mean predictions                  | (0.0317, 0.0452)  | (0.0317, 0.0451)  | .038391       | .03831       |
| Mean True Values                  | (0.0723, 0.0934)  | (0.0722, 0.0932)  | .0827777      | .08277       |
| Mean RMSE (True - Pred)           | (-0.0067, 0.0062) | (-0.0068, 0.0061) | -6.675433e-05 | -9.38212e-05 |
| Calibration                       | (0.0013, 0.0096)  | (0.0012, 0.0097)  | .00541        | .0053548     |

***Implications***
-Error being significant means that there is a significant difference between the true values and the BKT predictions. The same can be true for those in *only* the nonemerging group or in the emerging group.

-The mean predictions across both conditions being significant means that there is a significant difference between the predictions the model is giving. Similarly, we are also showing that there is significance in the base rates of the two groups as well.

-Having there not being a significant difference between the RMSE means that the distribution of errors between the two groups is not significant.

-Could mean that the model is splitting the difference between emerging and non-emerging readers. The overall RMSE is not capturing that due to it not capturing the direction of the error.
	-Could just look at the mean error for emerging readers vs nonemerging readers.
	 -mean error across all (calibration)
	 -aggregation causes continuous values
-report 4 decimal places for CI. 4000 decimal points


 Not to me...the previous part of the paragraph is talking about how fair the BKT model is, then here we conclude it is unfair. The unfairness is small, but it is there *in some ways*. Not RMSE, but others. Teasing apart this difference is critical, because it is theoretically impossible for it to be fair in every way if the base rates differ (which they do). This paragraph probably needs to bring up this very nuanced point, which is honestly close to the #1 takeaway from the paper for me (or #2 after reading skill is important). What kind of fairness do we want? Equal predicted rates of mastery, or equally correct predictions? Can't have it both ways, and the implications for education are enormous. And it is a touchy subject -- that's what affirmative action in college admissions debates are partly about.