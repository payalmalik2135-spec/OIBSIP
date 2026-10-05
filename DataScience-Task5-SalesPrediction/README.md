# Sales Prediction Using Python

**Oasis Infobyte SIP — Data Science Track (Task 5)**

## Objective
Build a regression model that predicts product sales based on advertising spend
across three media channels: TV, Radio, and Newspaper.

## Tech Stack
- Python
- pandas
- scikit-learn
- matplotlib / seaborn
- Jupyter Notebook

## What This Project Does
1. Loads the Advertising dataset (200 campaigns, 3 ad spend channels + Sales)
2. Performs exploratory data analysis (shape, data types, missing value check, descriptive statistics)
3. Visualizes relationships between ad spend and sales using pairplots, scatter plots, and a correlation heatmap
4. Splits the data into training (80%) and testing (20%) sets
5. Trains two regression models: **Linear Regression** and **Gradient Boosting Regressor**
6. Evaluates both models using MAE, RMSE, and R² score
7. Analyzes feature importance to determine which ad channel drives sales the most

## Results
| Model | MAE | RMSE | R² Score |
|---|---|---|---|
| Linear Regression | 1.14 | 1.56 | 0.91 |
| Gradient Boosting | 0.53 | 0.65 | 0.98 |

**Best model: Gradient Boosting Regressor**, achieving a 98% R² score — roughly half the
prediction error of Linear Regression.

### Key Findings
- **TV ad spend has the strongest impact on sales** — confirmed through correlation
  analysis (0.78), scatter plot trends, and feature importance ranking.
- **Radio ad spend has a moderate impact** (correlation 0.58).
- **Newspaper ad spend has minimal impact on sales** (correlation 0.23).

### Business Recommendation
Prioritizing **TV advertising** would likely yield the strongest returns, followed by
Radio. Newspaper spend contributes little to sales and could be reduced or reallocated.

## How to Run
1. Clone this repository or download the notebook
2. Install dependencies: `pip install pandas numpy scikit-learn matplotlib seaborn`
3. Open `sales_prediction.ipynb` in Jupyter Notebook or VS Code
4. Run all cells in order

## Author
Payal Malik — Data Science Intern, Oasis Infobyte
