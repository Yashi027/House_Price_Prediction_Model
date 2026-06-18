# House Price Prediction Model
## Objective
Traditional property valuation relies on manual, subjective comparison. This project builds and benchmarks regression models that estimate house prices from measurable housing features — replacing guesswork with a repeatable, data-driven pricing tool for real estate decision-making.
## Approach
Linear Regression was used as a baseline model assuming a linear relationship between features and price. Random Forest Regressor, an ensemble of decision trees, was tested to capture more complex, non-linear feature interactions.
## Model Evaluation
| Model | MAE | RMSE | R² Score |
|--------|------------:|------------:|---------:|
| Linear Regression | 970,043 | 1,324,507 | 0.653 |
| Random Forest Regressor | 1,009,617 | 1,389,518 | 0.618 |

Linear Regression outperformed the ensemble model, explaining about 65% of price variance suggesting the underlying price structure is largely additive rather than driven by complex feature interactions.
## Key Insights
Property area, bathrooms, stories, parking, preferred location, and air conditioning emerged as the strongest price drivers. Amenities and location rivaled structural features in influence — a furnished, well-located property can outprice a larger but plain one. Notably, the simpler model won: Random Forest's added complexity did not translate into better accuracy on this dataset, reinforcing that interpretable models remain valuable in real estate analytics. The unexplained variance (~35%) points to external factors absent from the dataset — neighbourhood reputation, economic conditions, and buyer sentiment.
