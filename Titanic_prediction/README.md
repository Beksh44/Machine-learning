👉 [View full prediction notebook (hosted via nbviewer)](
https://nbviewer.org/github/Beksh44/Machine-learning/blob/main/Titanic_prediction/prediction.ipynb
)

### Titanic Passenger Survival Prediction

This project focuses on predicting the survival of Titanic passengers using classification models. Training data is provided in the `data.csv` file, and evaluation data for testing predictions is found in `evaluation.csv`.

---

### 🔍 Feature Overview

The dataset includes the following features:

- `survived` – whether the passenger survived (0 = No, 1 = Yes); this is the **target variable**
- `pclass` – ticket class (1 = First, 2 = Second, 3 = Third)
- `name` – name of the passenger
- `sex` – gender
- `age` – age in years
- `sibsp` – number of siblings/spouses aboard
- `parch` – number of parents/children aboard
- `ticket` – ticket number
- `fare` – ticket fare
- `cabin` – cabin number
- `embarked` – port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)
- `home.dest` – home/destination

---

### 🧹 Data Preprocessing

To prepare the data for modeling, I went through the following steps:

- Transformed raw features into formats suitable for machine learning models
- Created new features based on existing ones (e.g., title extracted from name)
- Removed irrelevant or redundant features
- Dealt with missing values using simple but effective techniques
- Explored and visualized the data to better understand relationships between features

---

### 🤖 Modeling

I applied and evaluated two classification models:

- **Decision Tree**
- **K-Nearest Neighbors (KNN)**

For each model:

- I considered whether the model was suitable for this classification task
- Tuned key hyperparameters to improve performance
- Selected the best model based on F1 score and ROC-AUC evaluation
- Interpreted the results and compared model performance

---

### 🏁 Final Model and Prediction

After evaluating both models, I selected the one with the best performance as the final model. This model was used to predict survival on the unseen dataset (`evaluation.csv`).

The predictions were saved in a new file called `results.csv`, with the following format:


