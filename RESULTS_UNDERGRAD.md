
T = True
P = Predicted
D = DisparateRemover Predicted

Groups = Difference between groups

Math Data

	Overall RMSE (True - Pred): (0.0646, 0.0682)   |DR: (0.0645, 0.0680)
	RMSE (True - Pred) NonEmerge: (0.0638, 0.0675) |DR: (0.0638, 0.0674)
	RMSE (True - Pred) Emerging: (0.0642, 0.0736)  |DR: (0.0640, 0.0731)

| Comparison (Priv - NonPriv) | CI (95%) | DR  | Emerge (RW) |
| --------------------------- | -------- | --- | ----------- |
| Mean True Value             |          |     |             |
| Mean Predictions            |          |     |             |
| Mean RMSE (True - Pred)     |          |     |             |
| Calibration                 |          |     |             |







| DATASET | Model | Statistic          | CI                  |
| ------- | ----- | ------------------ | ------------------- |
| Math    | LR    | T Val (Groups)     | (-0.1697,  0.0277 ) |
| Math    | LR    | P Val (Groups)     | (-0.0695, -0.0034 ) |
| Math    | LR    | D Val (Groups)     | (-0.0584,  0.0075 ) |
| Math    | LR    | RMSE (T-P)         | ( 0.4826,  0.5325 ) |
| Math    | LR    | RMSE (T-D)         | ( 0.0530,  0.0871 ) |
| Math    | LR    | RMSE(T-P) (Groups) | (-0.0757,  0.0242 ) |
| Math    | LR    | RMSE(T-D) (Groups) | (-0.0875,  0.0220 ) |
| Math    | RF    | T Val (Groups)     | (-0.1692,  0.0275 ) |
| Math    | RF    | P Val (Groups)     | (-0.0687, -0.0026 ) |
| Math    | RF    | D Val (Groups)     |                     |
| Math    | RF    | RMSE (T-P)         | ( 0.4820,  0.5333 ) |
| Math    | RF    | RMSE (T-D)         | ( 0.4927,  0.5466 ) |
| Math    | RF    | RMSE(T-P) (Groups) | (-0.0743,  0.0258 ) |
| Math    | RF    | RMSE(T-D) (Groups) | (-0.0821,  0.0249 ) |

Research Questions:

Are generalizable unfairness mitigation strategies applicable in reducing gender bias in grade prediction?

Is there a significant difference in model statistics when unfairness mitigation is applied?