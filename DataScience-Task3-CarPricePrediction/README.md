# Car Price Prediction with Machine Learning

**Oasis Infobyte SIP — Data Science Track (Task 3)**

## Objective
Build a regression model that predicts the selling price of a used car from features such as
brand, age, kilometres driven, fuel type, transmission and number of previous owners.

## Dataset
CarDekho used car listings (`CAR DETAILS FROM CAR DEKHO.csv`) — 4,340 listings, 3,577 after
removing duplicates.

## Tech Stack
- Python
- pandas / numpy
- scikit-learn
- matplotlib / seaborn
- Jupyter Notebook

## What This Project Does
1. Loads the dataset and checks data quality (missing values, duplicates, data types)
2. Removes 763 duplicate listings and cleans text columns
3. Engineers new features: **car age** (from the manufacture year) and **brand** (from the car name)
4. Explores the data with a price histogram, price by fuel type, price vs car age and average price by brand
5. Encodes categorical columns with one-hot encoding and plots a feature correlation heatmap
6. Splits the data into training (80%) and testing (20%) sets
7. Trains two regression models: **Linear Regression** and **Random Forest Regressor**
8. Evaluates both models using MAE, RMSE and R² score
9. Plots feature importance for the best model

## Results
| Model | MAE (₹ lakh) | RMSE (₹ lakh) | R² Score |
|---|---|---|---|
| Linear Regression | 1.75 | 3.92 | 0.58 |
| Random Forest | 1.58 | 4.00 | 0.56 |

**Best model: Linear Regression** — highest R² and lowest RMSE, though the two models are close.

### Key Findings
- Transmission type and car age are the strongest factors: manual cars and older cars sell for less.
- Brand has a large effect: luxury brands (Audi, Mercedes-Benz, BMW) raise the predicted price,
  while budget brands (Maruti, Tata, Hyundai, Chevrolet) lower it.
- Diesel cars tend to sell for more than petrol cars.

### Limitations
- A few very expensive luxury cars are hard to predict, which keeps R² moderate.
- The dataset has no engine size, power or condition information.

## How to Run
1. Download this folder (notebook and CSV file)
2. Install dependencies: `pip install pandas numpy scikit-learn matplotlib seaborn`
3. Open `car_price_prediction.ipynb` in Jupyter Notebook or VS Code
4. Run all cells in order

## Author
Payal Malik — Data Science Intern, Oasis Infobyte
