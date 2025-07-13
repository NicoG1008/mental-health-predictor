# Mental Health & Lifestyle Predictor

This project explores how daily habits and lifestyle choices—like diet, exercise, screen time, and sleep—may correlate with self-reported mental health conditions. Using machine learning models (Random Forest and XGBoost), we attempt to predict whether an individual reports a mental health condition based on survey data.

---

## Motivation

As someone passionate about health and data science, I created this project to:
- Explore how lifestyle factors relate to mental health
- Learn and apply machine learning techniques
- Build a practical, portfolio-ready project in Python

---

## Dataset

- **Source**: Mental Health & Lifestyle Survey Dataset (Kaggle - Atharva Soundankar - "Mental Health and Lifestyle Habits (2019-2024)")
- **Size**: ~3,000 responses
- **Key Features Used**:
  - Sleep Hours  
  - Screen Time  
  - Work Hours  
  - Social Interaction Score  
  - Diet Type  
  - Stress Level  
  - Exercise Level

- **Target Variable**: Binary classification — whether the participant self-reports a mental health condition (vs. none)

---

## Tools & Libraries

- Python (Colab Notebook)
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Seaborn, Matplotlib

---

## Modeling Summary

Three models were tested:

| Model              | Accuracy | Notes |
|-------------------|----------|-------|
| Logistic Regression | ~0.54     | Baseline |
| Random Forest       | ~0.57     | Best with `n_estimators=10`, `max_depth=6–10` |
| XGBoost             | ~0.54    | Efficient but slightly worse than Random Forest |

**Top Predictive Features**:
- Stress level
- Exercise level
- Diet type (vegetarian, vegan, keto, balanced, junk food)

---

## Key Takeaways

- Lifestyle factors, especially stress, diet, and exercise, show predictive value for self-reported mental health conditions.
- Simple models can perform competitively when the dataset is small or noisy.
- Feature importance helps interpret the role of daily habits in mental well-being.

---

## How to Run This Project

You can open the project directly in Google Colab [https://colab.research.google.com/drive/1K6rtcmOhYRQNGfjJxZjndhBNMIRBKgUH?usp=sharing] 

### Steps:
1. Upload the dataset or read it with `pd.read_csv()`
2. Run the notebook from top to bottom
3. Modify features, models, or hyperparameters to experiment

---

## Limitations

- Self-reported data may include bias or noise
- The target variable is not a clinical diagnosis
- The dataset is modest in size and class-imbalanced

---

## Future Improvements

- Apply resampling methods like SMOTE to balance the dataset
- Use SHAP or LIME to interpret predictions more deeply
- Explore more advanced models or neural networks
- Build an interactive Streamlit app for public input and prediction

---

## About Me

I'm an undergraduate biology-chemistry major with a passion for exercise science, nutrition, psychology, and data. This project blends academic and personal interests into an accessible machine learning analysis.

---
