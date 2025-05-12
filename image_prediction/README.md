# 🧥 Image Classification

This project focuses on classifying grayscale images of clothing items (e.g., coats, dresses) using various machine learning algorithms. The dataset contains 28x28 pixel images and is used to explore the performance of classifiers under different conditions and preprocessing strategies.

---

## 📊 Goal

The primary objective is to predict the correct class of a clothing item from pixel data using different models and preprocessing strategies. The final model is selected based on its performance on validation data and tested on `evaluate.csv`.

---

## 🔧 Models and Methods Used

### 🧠 Classifiers:
- **Support Vector Machine (SVM)**
- **Naive Bayes (GaussianNB)**
- **Linear Discriminant Analysis (LDA)**

### 🔍 Dimensionality Reduction:
- **Principal Component Analysis (PCA)**
- **Locally Linear Embedding (LLE)**

Each model is tested with:
- Original data (no reduction)
- PCA-reduced data (10, 50, 100 dimensions)
- LLE-reduced data (3, 5, 8 dimensions)

---

## 🥇 Final Model Selection

| Model            | Dimensionality | Best Accuracy |
|------------------|----------------|----------------|
| **SVM**          | No reduction   | **0.96** ✅ |
| Naive Bayes      | LLE (dim=3)    | 0.88          |
| Naive Bayes      | No reduction   | 0.87          |
| LDA              | No reduction   | 0.93          |

**✅ SVM without dimensionality reduction** was selected as the final model due to the highest validation accuracy of **0.96**.
