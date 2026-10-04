# Iris Flower Classification

**Oasis Infobyte SIP — Data Science Track (Task 1)**

## Objective
Train a machine learning model to classify iris flowers into one of three species
(*Setosa*, *Versicolor*, or *Virginica*) based on their physical measurements:
sepal length, sepal width, petal length, and petal width.

## Tech Stack
- Python
- pandas
- scikit-learn
- matplotlib / seaborn
- Jupyter Notebook

## What This Project Does
1. Loads the built-in Iris dataset from scikit-learn
2. Performs exploratory data analysis (shape, data types, missing value check, descriptive statistics)
3. Visualizes relationships between features using a pairplot and box plots
4. Splits the data into training (80%) and testing (20%) sets
5. Trains two classification models: **Logistic Regression** and **K-Nearest Neighbours (KNN)**
6. Evaluates both models using accuracy, confusion matrices, and classification reports
7. Compares the models and identifies the best performer

## Results
| Model | Accuracy |
|---|---|
| Logistic Regression | 96.67% |
| K-Nearest Neighbours (KNN) | 100% |

**Best model: K-Nearest Neighbours (KNN)**, achieving perfect accuracy on the test set.

### Key Findings
- Petal length and petal width are far more useful for distinguishing species than sepal measurements.
- *Setosa* is fully separable from the other two species.
- *Versicolor* and *Virginica* have some overlap, which accounted for the one misclassification Logistic Regression made.

## How to Run
1. Clone this repository or download the notebook
2. Install dependencies: `pip install pandas numpy scikit-learn matplotlib seaborn`
3. Open `iris_classification.ipynb` in Jupyter Notebook or VS Code
4. Run all cells in order

## Author
Payal Malik — Data Science Intern, Oasis Infobyte
