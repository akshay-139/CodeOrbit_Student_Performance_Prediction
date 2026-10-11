# 🎓 Student Performance Analysis and Prediction

A beginner-friendly Machine Learning project that analyzes student performance data and uses classification and regression models to explore student outcomes.

## 📌 Project Overview

This project uses the **Student Performance dataset from the UCI Machine Learning Repository** to explore factors related to students' academic performance.

It includes exploratory data analysis (EDA), a Pass/Fail classification model, and a regression model to predict final grades.

## 🎯 Objectives

- Understand and analyze student performance data.
- Inspect missing values, duplicate records, and numerical statistics.
- Visualize the distribution of final grades and relationships between selected features.
- Classify students as Pass or Fail.
- Predict students' final grades using Machine Learning.

## 📊 Dataset

- **Source:** UCI Machine Learning Repository
- **Dataset:** Student Performance
- **Number of records:** 649
- **Number of columns:** 33, including input features and grade targets
- **Final grade column:** `G3`

For this project, a student is classified as:
- **Pass:** Final grade (`G3`) ≥ 10
- **Fail:** Final grade (`G3`) < 10

Dataset source: https://archive.ics.uci.edu/dataset/320/student+performance

## 🛠️ Technologies Used

- **Python** — Programming language
- **Pandas** — Data handling and analysis
- **NumPy** — Numerical operations
- **Matplotlib** — Data visualization
- **Seaborn** — Correlation heatmap
- **Scikit-learn** — Machine Learning models and evaluation metrics
- **Jupyter Notebook / Google Colab** — Development environment

## 🔍 Project Workflow

1. Loaded the dataset and combined the input features with grade targets.
2. Inspected the data using `info()`, `describe()`, and missing-value and duplicate checks.
3. Performed exploratory data analysis using histograms, scatter plots, boxplots, bar charts, and a correlation heatmap.
4. Built a Logistic Regression model to classify Pass and Fail outcomes.
5. Built a Linear Regression model to predict final grades.
6. Evaluated the models using appropriate performance metrics.

## 🤖 Machine Learning Models

### 1. Pass/Fail Classification

- **Algorithm:** Logistic Regression
- **Input features:** Age, study time, previous failures, and absences
- **Target:** Pass or Fail based on the final grade (`G3`)
- **Evaluation metrics:** Accuracy, Precision, and Recall

### 2. Final Grade Prediction

- **Algorithm:** Linear Regression
- **Input features:** Age, study time, previous failures, and absences
- **Target:** Final grade (`G3`)
- **Evaluation metrics:** Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE)

The models use four selected features and do not use the earlier grades `G1` and `G2` as inputs.

## 📈 Results

| Metric | Result |
|---|---:|
| Classification Accuracy | 83.85% |
| Classification Precision | 85.04% |
| Classification Recall | 98.18% |
| Regression MAE | 2.21 marks |
| Regression RMSE | 2.88 marks |

**Interpretation:** The classification model achieved 83.85% accuracy on the test set. The regression model's predictions differed from actual grades by about 2.21 marks on average in absolute terms.

These results apply to this particular dataset split and should not be treated as a guarantee of performance on other student groups.

## 💡 Key Learnings

- Data inspection and basic data-quality checks
- Exploratory Data Analysis and visualization
- Preparing features and target variables
- Training classification and regression models
- Evaluating models using classification and regression metrics
- Understanding the limitations of Machine Learning predictions

## ▶️ How to Run the Project

1. Open `Student_Performance.ipynb` in Google Colab or Jupyter Notebook.
2. Install the required libraries if they are not already available.
3. Run the notebook cells in order.
4. Review the generated visualizations, model metrics, and actual-versus-predicted grade plot.

Install the dataset package if needed:

```bash
pip install ucimlrepo
```

## ⚠️ Limitations

- Only four selected input features are used for the models.
- The dataset and test split are limited, so the results may differ on other data.
- The predictions are estimates and should not be used as definitive judgments about individual students.
- Relationships observed in the data do not necessarily imply causation.

## 👨‍💻 Author

Akshay Kumar Singh

---

