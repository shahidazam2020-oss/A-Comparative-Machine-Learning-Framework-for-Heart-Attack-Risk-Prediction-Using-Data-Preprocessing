# 🫀 A Comparative Machine Learning Framework for Heart Attack Risk Prediction

<p align="center">

### 🤖 Machine Learning • Healthcare Analytics • Predictive Modeling • Clinical Risk Prediction

A systematic machine learning framework integrating data preprocessing, class-imbalance handling, hyperparameter optimization, and five-fold cross-validation for heart attack risk prediction.

</p>

---

## 📌 Research Overview

Cardiovascular diseases and heart attacks remain major healthcare challenges worldwide. Early identification of individuals at risk can support timely intervention and improved healthcare decision-making.

This research develops a **comparative machine learning framework for heart attack risk prediction** by combining systematic data preprocessing, feature preparation, class-imbalance handling, hyperparameter optimization, and cross-validation.

Multiple supervised machine learning algorithms are evaluated to determine their effectiveness in predicting heart attack risk and identifying high-risk cases.

The study emphasizes that **accuracy alone is not sufficient for evaluating healthcare prediction models**, particularly when correctly identifying positive/risk cases is clinically important.

---

# 🎯 Research Objectives

**The main objectives of this research are to:**

* 🫀 Develop a machine learning framework for heart attack risk prediction
* 🧹 Apply systematic data preprocessing
* 🔍 Identify relevant predictive features
* ⚖️ Address class imbalance using SMOTE and class weighting
* 🤖 Compare multiple machine learning algorithms
* ⚙️ Optimize model hyperparameters
* 🔄 Apply five-fold cross-validation
* 📊 Evaluate models using multiple performance metrics
* 🎯 Investigate minority-class/heart-attack detection
* 🏆 Identify models with the most useful predictive characteristics

---

# 📊 Dataset

*The research uses a **Heart Attack Risk Prediction Dataset obtained from Kaggle**.*

The target variable is:

```text
Heart Attack Risk
```

**It is treated as a binary classification problem:**

```text
1 → Heart Attack Risk
0 → No Heart Attack Risk
```

**The study considers demographic, physiological, lifestyle, and clinical-related variables. Examples include:**

* Age
* Sex
* Cholesterol
* Systolic blood pressure
* Diastolic blood pressure
* Smoking
* Diabetes
* Family history
* Obesity
* Alcohol consumption
* Exercise
* BMI
* Stress level
* Previous heart problems
* Physical activity
* Sleep
* Other patient-related characteristics

**The research methodology describes the target as a binary dependent variable and identifies age, sex, cholesterol, blood pressure, smoking, and diabetes among the predictor variables.**

---

# 🔬 Research Methodology

**The study follows a quantitative machine-learning research methodology.**

```text
                  🫀 HEART ATTACK DATA
                          │
                          ▼
                  🧹 DATA PREPROCESSING
                          │
            ┌─────────────┴─────────────┐
            │                           │
            ▼                           ▼
      Missing Values              Data Cleaning
      Duplicates                  Outliers
      Inconsistencies             Feature Preparation
            │                           │
            └─────────────┬─────────────┘
                          ▼
                  🔍 FEATURE SELECTION
                          │
                          ▼
                  ⚖️ CLASS BALANCING
                          │
                ┌─────────┴─────────┐
                ▼                   ▼
              SMOTE          Class Weighting
                │                   │
                └─────────┬─────────┘
                          ▼
                  🤖 MODEL TRAINING
                          │
                          ▼
               ⚙️ HYPERPARAMETER
                  OPTIMIZATION
                          │
                          ▼
                 🔄 5-FOLD CV
                          │
                          ▼
                  📊 MODEL EVALUATION
                          │
          ┌───────────────┼───────────────┐
          ▼               ▼               ▼
       Accuracy         Recall          F1
          │               │               │
          └───────────────┼───────────────┘
                          ▼
                     🏆 COMPARISON
```

**The dataset was divided into **80% training and 20% testing data**, followed by five-fold cross-validation for more robust performance estimation and reduced overfitting risk.**

---

# 🧹 Data Preprocessing

**Before model development, the dataset was examined for:**

* Missing values
* Duplicate records
* Inconsistent observations
* Potential outliers
* Data quality issues

*Descriptive statistics were used to understand the characteristics of the dataset before model development.*

*Feature selection was subsequently performed to identify variables considered most relevant to heart attack prediction.*

---

# ⚖️ Class Imbalance Handling

Class imbalance is an important issue in healthcare machine learning because models may become biased toward the majority class.

The research incorporates **Synthetic Minority Oversampling Technique (SMOTE)** and **class weighting** to improve the representation and detection of heart attack cases.

### 🔵 Original Distribution

**The dataset contained:**

```text
2511 → No Heart Attack Risk
2511 → Heart Attack Risk

Total = 5022 observations
```

**The original classes were therefore balanced in the analyzed dataset.**

### 🟣 SMOTE Distribution

After SMOTE:

```text
4499 → Class 0
4499 → Class 1
```

*SMOTE increased the training representation to provide a larger balanced training set.*

---

# 🤖 Machine Learning Models

**The research compares multiple supervised machine learning algorithms.**

## 1. 📈 Logistic Regression

Used as the baseline classification model because of its simplicity, computational efficiency, and interpretability.

---

## 2. 🌲 Random Forest

An ensemble learning algorithm capable of modeling nonlinear relationships.

It combines predictions from multiple decision trees to improve robustness and reduce variance.

---

## 3. 🌳 Decision Tree

A tree-based classification model used to analyze nonlinear relationships and improve detection of heart attack cases.

---

## 4. 🚀 Gradient Boosting

An ensemble technique that sequentially builds models to improve predictive performance.

---

## 5. ⚡ LightGBM

A gradient-boosting framework designed for efficient and scalable tree-based learning.

---

## 6. 🔥 AdaBoost

An adaptive boosting algorithm that gives greater importance to observations incorrectly classified by previous learners.

---

## 7. 🧠 MLP Neural Network

A Multi-Layer Perceptron neural network used to investigate whether nonlinear neural-network modeling can capture complex relationships between patient characteristics and heart attack risk.

The paper describes the rationale for using these models as a comparative framework, including Random Forest for nonlinear relationships, boosting algorithms for structured healthcare data, and MLP for complex nonlinear interactions.

---

# ⚙️ Hyperparameter Optimization

Hyperparameter optimization was performed to identify appropriate configurations for the machine learning algorithms.

The optimization process was integrated with model validation to improve predictive performance and reduce the likelihood of selecting models based only on a single train/test split.

The final framework therefore combines:

```text
Model
  ↓
Hyperparameter Optimization
  ↓
Cross-Validation
  ↓
Best Configuration
  ↓
Final Evaluation
```

---

# 🔄 Five-Fold Cross-Validation

*The study applies **5-fold cross-validation***

```text
Fold 1 → Train / Validate
Fold 2 → Train / Validate
Fold 3 → Train / Validate
Fold 4 → Train / Validate
Fold 5 → Train / Validate
          ↓
   Average Performance
```

*This allows the models to be repeatedly trained and validated on different subsets of the data.*

**The objective is to obtain a more reliable estimate of model performance and reduce the risk of overfitting.**

---

# 📊 Evaluation Metrics

**Multiple metrics are used because healthcare prediction requires more than simply measuring overall accuracy.**

### 🎯 Accuracy

Measures the proportion of correctly classified observations.

### 🔎 Precision

Measures how many observations predicted as positive were actually positive.

### ❤️ Recall

Measures how many actual heart attack-risk cases were correctly identified.

### ⚖️ F1-Score

Combines precision and recall into a single metric.

### 📈 ROC-AUC

Measures the model's ability to distinguish between positive and negative classes.

### 🧩 Confusion Matrix

Provides detailed counts of:

* True Positives
* True Negatives
* False Positives
* False Negatives

**The paper explicitly evaluates accuracy, precision, recall, F1-score, ROC-AUC, balanced accuracy, and confusion matrices.**

---

# 🏆 Key Results

**The experiments demonstrate that different models perform better under different evaluation criteria.**

| Model                  | Approx. Accuracy | Key Observation                    |
| ---------------------- | ---------------: | ---------------------------------- |
| 🥇 Random Forest       |         **~64%** | Best overall accuracy              |
| 🥈 Logistic Regression |         **~64%** | Strong overall classification      |
| 🥉 Gradient Boosting   |         **~63%** | Strong ensemble performance        |
| ⚡ LightGBM             |         **~62%** | Strong overall performance         |
| 🌳 Decision Tree       |         **~54%** | Better minority-class detection    |
| 🧠 MLP Neural Network  |         **~54%** | Better heart-attack case detection |

**The reported results show Random Forest and Logistic Regression achieving approximately 0.64 accuracy, while Gradient Boosting and LightGBM achieved above 0.62.**

---

# ❤️ Minority-Class Detection

One of the most important findings is that **the model with the highest accuracy was not necessarily the best at detecting heart attack-risk cases**.

The Decision Tree and MLP Neural Network achieved higher F1-scores and recall than several other models.

Reported F1-scores were approximately:

```text
🌳 Decision Tree       → 0.37
🧠 MLP Neural Network  → 0.34
⚡ LightGBM             → 0.12
📈 Logistic Regression → <0.05
🌲 Random Forest        → <0.05
🚀 Gradient Boosting    → <0.05
```

This demonstrates why relying exclusively on accuracy can be misleading in healthcare prediction.

---

# 🔥 Random Forest Performance

Random Forest achieved approximately:

```text
Accuracy  → 0.643
Precision → 0.494
```

**It produced the strongest overall positive-class accuracy and precision among the compared models in the reported experiment.**

---

# 🧠 MLP Neural Network Performance

The MLP demonstrated an important advantage in detecting heart attack-risk cases.

Its confusion matrix showed:

```text
❤️ Correct Risk Cases       → 215
✅ Correct Non-Risk Cases   → 725
❌ Risk → Non-Risk          → 413
❌ Non-Risk → Risk          → 400
```

**Compared with LightGBM, the MLP correctly detected substantially more heart attack-risk cases in the reported experiment.**

This suggests a trade-off between **sensitivity and specificity** that is particularly important in healthcare applications.

---

# 📈 ROC-AUC Results

The reported ROC-AUC values were relatively close to random classification:

```text
🌲 Random Forest        → ~0.52
⚡ LightGBM              → ~0.51
🚀 Gradient Boosting    → ~0.51
📈 Logistic Regression  → ~0.50
🌳 Decision Tree        → ~0.50
🧠 MLP                  → ~0.47
```

These results indicate that the models had **limited class-separation capability** on the evaluated dataset, despite differences in accuracy and F1-score.

---

# 🔄 Cross-Validation Results

**The five-fold cross-validation results reported approximately:**

```text
Accuracy  → 60%
Precision → 35%
Recall    → 13%
F1-Score  → 19%
```

This provides an additional view of model generalizability across different folds.

---

# 💡 Main Research Findings

### 🥇 Best Overall Classification

**Random Forest and Logistic Regression** achieved the strongest overall accuracy, around 64%.

### ❤️ Best Heart Attack Detection

**Decision Tree and MLP Neural Network** demonstrated stronger minority-class detection through higher recall and F1-score.

### ⚡ Ensemble Performance

Gradient Boosting and LightGBM achieved competitive overall accuracy above 62%.

### 📊 Accuracy Is Not Enough

A model can achieve high overall accuracy while failing to detect a substantial number of actual heart attack-risk cases.

### 🔄 Cross-Validation Matters

Five-fold cross-validation provides a more robust assessment of model generalization.

These findings support the paper's conclusion that **no single model is best across every evaluation criterion**.

---

# 🧠 Research Contribution

*The key contribution of this research is the development of a **systematic and repeatable machine-learning framework** that combines:*

```text
🧹 Data Preprocessing
        +
🔍 Feature Selection
        +
⚖️ Class Imbalance Handling
        +
⚙️ Hyperparameter Optimization
        +
🔄 Five-Fold Cross-Validation
        +
📊 Multi-Metric Evaluation
        ↓
🫀 Heart Attack Risk Prediction
```

**Rather than evaluating machine learning algorithms using accuracy alone, the framework emphasizes the importance of **recall, precision, F1-score, ROC-AUC, and confusion matrices**, especially for identifying high-risk cases.**

---

# 🛠️ Technologies Used

| Technology          | Purpose                         |
| ------------------- | ------------------------------- |
| 🐍 Python           | Machine learning implementation |
| 🐼 Pandas           | Data processing                 |
| 🔢 NumPy            | Numerical operations            |
| 🤖 Scikit-learn     | Machine learning                |
| ⚖️ Imbalanced-learn | SMOTE/class balancing           |
| 📊 Matplotlib       | Visualization                   |
| 🎨 Seaborn          | Statistical visualization       |
| 📈 Plotly           | Interactive visualization       |
| 📋 SPSS             | Statistical analysis            |
| 📓 Jupyter Notebook | Experimentation                 |

---

# 📁 Repository Structure

```text
Heart-Attack-Risk-Prediction/
│
├── 📄 Research-Paper.docx
├── 📄 Research-Paper.pdf
├── 📓 notebooks/
│   ├── preprocessing.ipynb
│   ├── model_training.ipynb
│   └── evaluation.ipynb
│
├── 📊 results/
│   ├── confusion_matrices/
│   ├── model_comparison/
│   ├── roc_curves/
│   └── cross_validation/
│
├── 🖼️ figures/
│
└── README.md
```

---

# 🚀 Research Workflow

```text
          DATASET
             │
             ▼
     🧹 PREPROCESSING
             │
             ▼
      🔍 FEATURE SELECTION
             │
             ▼
       ⚖️ SMOTE / WEIGHTS
             │
             ▼
     🤖 7 ML ALGORITHMS
             │
             ▼
    ⚙️ HYPERPARAMETER TUNING
             │
             ▼
       🔄 5-FOLD CV
             │
             ▼
     📊 MULTI-METRIC TESTING
             │
             ▼
       🏆 COMPARATIVE
          ANALYSIS
             │
             ▼
      🫀 HEART ATTACK
       RISK PREDICTION
```

---

# 📌 Repository Purpose

**This repository provides the research materials and supporting resources for the study:**

> **“A Comparative Machine Learning Framework for Heart Attack Risk Prediction Using Data Preprocessing, Class Imbalance Handling, and Cross-Validation.”**

The repository is intended to support:

* 🎓 Academic research
* 🔬 Reproducible experimentation
* 🤖 Machine learning research
* 🫀 Healthcare analytics
* 📊 Predictive modeling
* 📚 Further research and extension

---

# ⚠️ Important Research Disclaimer

This project is intended for **academic and research purposes**. The machine-learning models presented in this study are experimental predictive models and **are not intended to replace professional medical diagnosis, clinical judgment, or validated clinical decision-support systems**.

**The reported results are based on the dataset and experimental methodology described in the research paper.**

---

# 👨‍🔬 Authors

### **Dr. Adnan Amin**

### **Shahid Azam**

**Research Area:** Machine Learning • Healthcare Analytics • Cardiovascular Risk Prediction • Predictive Modeling

---

# 📚 Citation

If you use this research or repository in your work, please cite:

```text
Amin, A., & Azam, S. (2026).
A Comparative Machine Learning Framework for Heart Attack Risk Prediction
Using Data Preprocessing, Class Imbalance Handling, and Cross-Validation.
```

---

<p align="center">

### 🫀 Machine Learning for Smarter Healthcare

**Data → Intelligence → Prediction → Better Decision Support**

</p>
