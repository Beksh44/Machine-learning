### Life Expectancy Prediction

This project focuses on predicting life expectancy across different countries and years using regression models. The training data is provided in `data.csv`, and the evaluation data for generating predictions is found in `evaluation.csv`.

---

### 🌍 Dataset Overview

Each row represents health, demographic, and economic indicators for a given country and year. The goal is to predict:

- **Target variable**: `Life expectancy` – Life expectancy at birth (in years)

**Features include:**

- `Year` – Year of observation  
- `Status` – Developed or developing country  
- `Adult Mortality` – Adult mortality rate (age 15–60, per 1,000 people)  
- `infant deaths` – Number of infant deaths per 1,000 population  
- `Alcohol` – Alcohol consumption per adult (in litres)  
- `percentage expenditure` – Healthcare expenditure as % of GDP  
- `Hepatitis B` – HepB vaccination coverage for 1-year-olds (%)  
- `Measles` – Reported measles cases per 1,000 population  
- `BMI` – Average Body Mass Index of the population  
- `under-five deaths` – Child mortality under 5 years per 1,000  
- `Polio` – Polio vaccination coverage for 1-year-olds (%)  
- `Total expenditure` – Government health spending (% of total government spending)  
- `Diphtheria` – DTP3 vaccination coverage for 1-year-olds (%)  
- `HIV/AIDS` – Deaths due to HIV/AIDS per 1,000 live births  
- `GDP` – Gross Domestic Product per capita (USD)  

---

### 🧹 Data Preprocessing

After loading the data, I prepared it with a few key steps:

- Transformed features into formats suitable for regression models  
- Handled missing values using simple imputation strategies  
- Explored and visualized the data to identify patterns and relationships  
- Split the dataset into subsets for training, validation, and testing  

---

### 🌲 Random Forest Implementation

A custom implementation of the **Random Forest Regressor** was built and used as one of the core models. The provided structure was used as a base for this implementation.

---

### 📈 Model Training and Comparison

After preprocessing, several models were trained and compared:

- ✅ My custom **Random Forest** implementation  
- ✅ Either **Linear Regression** or **Ridge Regression**  
- ✅ Optionally, another regression model of choice

For each model:

- I evaluated its suitability for this task  
- Experimented with normalization techniques (standardization or min-max)  
- Tuned key hyperparameters for optimal performance (based on RMSE)  
- Computed RMSE and MAE on the validation set  
- Documented and interpreted all results  

---

### 🏁 Final Prediction and Output

After evaluating model performance, I selected the final model and used it to predict life expectancy on the `evaluation.csv` data.

The predictions were saved in a file called `results.csv`, formatted as follows:

Country,Year,Life expectancy
Peru,2012,71.4
Peru,2013,72.6
...
