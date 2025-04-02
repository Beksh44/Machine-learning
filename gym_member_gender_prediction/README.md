### Gym Members Exercise Prediction

This project aims to predict the **gender** of gym members based on their exercise behavior, body composition, and workout stats using classification models.

The dataset used is from Kaggle:  
[Gym Members Exercise Tracking Dataset](https://www.kaggle.com/datasets/valakhorasani/gym-members-exercise-dataset)

---

### 📊 Gym Members Dataset Overview

The dataset provides a detailed overview of gym members' exercise routines, physical attributes, and fitness metrics. It includes 973 samples, with key performance indicators such as heart rate, calories burned, and workout duration. Demographic data and experience levels are also available for deeper insight into fitness patterns.

#### 🔑 Key Features:

- `Age`: Age of the gym member  
- `Gender`: Target variable – Male or Female  
- `Weight (kg)`, `Height (m)`: Physical attributes  
- `Max_BPM`, `Avg_BPM`, `Resting_BPM`: Heart rate stats  
- `Session_Duration (hours)`, `Workout_Frequency (days/week)`: Workout behavior  
- `Calories_Burned`: Total burned during workout  
- `Workout_Type`: Type of exercise (Cardio, Strength, HIIT, Yoga, etc.)  
- `Fat_Percentage`, `Water_Intake (liters)`, `BMI`: Health-related metrics  
- `Experience_Level`: Skill level (1 = beginner, 3 = expert)

---

### 🎯 Predicting Gender

The goal is to predict the `Gender` variable, which is:

- `0` = female  
- `1` = male

This makes it a **classification problem**, where we aim to build a model that identifies patterns from features like `Workout_Type`, `Calories_Burned`, `Experience_Level`, and more to correctly classify gender.

---

### 🔍 Approach

1. **Data Preparation**  
   - Handled missing values  
   - Encoded categorical variables  
   - Scaled numerical features  

2. **Feature Selection**  
   - Identified key predictors (e.g., `Workout_Type`, `Workout_Frequency`, `Calories_Burned`)

3. **Modeling**  
   - Applied classification models (Random Forest, KNN, etc.)

4. **Evaluation**  
   - Used metrics like **accuracy**, **precision**, **recall**, and **F1-score**  
   - Applied **cross-validation** to ensure robust results and prevent overfitting

---

### ✅ Results

The final model was evaluated using standard classification metrics and was able to predict gender with reasonable accuracy based on workout-related features. Visualizations helped explain both feature importance and model behavior.

---


