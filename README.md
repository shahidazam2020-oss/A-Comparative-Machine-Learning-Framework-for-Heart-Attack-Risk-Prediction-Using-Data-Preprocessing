<div align="center">

# 🫀 A Comparative Machine Learning Framework for Heart Attack Risk Prediction

### Data Preprocessing • Class Imbalance Handling • Cross-Validation • Predictive Modeling

<p>
  <img src="https://img.shields.io/badge/Research-Machine%20Learning-blue?style=for-the-badge&logo=academia" />
  <img src="https://img.shields.io/badge/Domain-Healthcare%20AI-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Focus-Predictive%20Modeling-purple?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Language-Python-yellow?style=for-the-badge&logo=python&logoColor=white" />
</p>

<br>

<a href="https://github.com/shahidazam2020-oss/A-Comparative-Machine-Learning-Framework-for-Heart-Attack-Risk-Prediction-Using-Data-Preprocessing">
  <img src="https://img.shields.io/badge/📂_GitHub-Explore_Repository-181717?style=for-the-badge&logo=github" />
</a>

<a href="https://www.researchgate.net/publication/408266268_A_Comparative_Machine_Learning_Framework_for_Heart_Attack_Risk_Prediction_Using_Data_Preprocessing_Class_Imbalance_Handling_and_Cross-Validation">
  <img src="https://img.shields.io/badge/🔬_ResearchGate-Read_Publication-00CCBB?style=for-the-badge&logo=researchgate&logoColor=white" />
</a>

<br><br>

<a href="#-research-overview">Overview</a> • <a href="#-research-objectives">Objectives</a> • <a href="#-dataset-overview">Dataset</a> • <a href="#-research-methodology">Methodology</a> • <a href="#-key-findings">Findings</a> • <a href="#-connect-with-me">Connect</a>

</div>

---

# 📖 Research Overview

**Cardiovascular diseases and heart attacks remain significant global healthcare challenges. Early identification of individuals at risk can support timely medical intervention and improve healthcare decision-making.**

This research presents a comparative Machine Learning framework for predicting heart attack risk by integrating systematic data preprocessing, feature preparation, class imbalance handling, hyperparameter optimization, and five-fold cross-validation.

Seven supervised machine learning algorithms are investigated to compare their predictive capabilities and identify their strengths and limitations in healthcare risk prediction.

The research particularly emphasizes the importance of evaluating models beyond accuracy, considering metrics such as Recall, Precision, F1-Score, ROC-AUC, and Confusion Matrices.

> **Research Focus:** Developing and evaluating a systematic machine learning framework that emphasizes reliable heart attack risk prediction and minority-class detection.

---

# 🎯 Research Objectives

The primary objectives of this research include:

* 🫀 Developing a comparative machine learning framework for heart attack risk prediction.
* 🧹 Applying systematic data preprocessing and cleaning.
* 🔍 Identifying relevant predictive features.
* ⚖️ Addressing class imbalance using SMOTE and class weighting.
* 🤖 Comparing multiple supervised machine learning algorithms.
* ⚙️ Optimizing model hyperparameters.
* 🔄 Applying five-fold cross-validation.
* 📊 Evaluating predictive performance using multiple metrics.
* ❤️ Investigating minority-class detection capabilities.
* 🏆 Identifying the strengths and limitations of different models.

---

# 📊 Dataset Overview

The research utilizes the Heart Attack Risk Prediction Dataset obtained from Kaggle.

### 🎯 Target Variable

`Heart Attack Risk`

The prediction task is formulated as a binary classification problem.

| Target Value | Description          |
| :----------: | -------------------- |
|       0      | No Heart Attack Risk |
|       1      | Heart Attack Risk    |

### 🔍 Dataset Features

The dataset includes demographic, physiological, lifestyle, and clinical-related variables.

| Category          | Features                                          |
| :---------------- | :------------------------------------------------ |
| 👤 Demographic    | Age, Sex                                          |
| ❤️ Cardiovascular | Cholesterol, Systolic BP, Diastolic BP            |
| 🚬 Lifestyle      | Smoking, Alcohol Consumption, Exercise            |
| 🩺 Medical        | Diabetes, Family History, Previous Heart Problems |
| ⚖️ Physical       | BMI, Obesity                                      |
| 🧠 Other Factors  | Stress Level, Sleep, Physical Activity            |

### 📌 Dataset Information

| Property                    | Details                      |
| :-------------------------- | :--------------------------- |
| Dataset                     | Heart Attack Risk Prediction |
| Source                      | Kaggle                       |
| Problem Type                | Binary Classification        |
| Target Variable             | Heart Attack Risk            |
| Original Observations       | 5,022                        |
| Original Class Distribution | 2,511 per class              |

---

# 🔬 Research Methodology

The study follows a quantitative machine learning research methodology.

The proposed framework integrates data preprocessing, feature selection, class balancing, model development, optimization, and performance evaluation.

### 🧭 Research Workflow

```text
              🫀 HEART ATTACK DATASET
                         |
                         ▼
                🧹 DATA PREPROCESSING
                         |
                         ▼
                 🔍 FEATURE SELECTION
                         |
                         ▼
               ⚖️ CLASS IMBALANCE
                    HANDLING
                         |
                ┌────────┴────────┐
                ▼                 ▼
              SMOTE         CLASS WEIGHTING
                └────────┬────────┘
                         |
                         ▼
                🤖 MODEL TRAINING
                         |
                         ▼
              ⚙️ HYPERPARAMETER
                  OPTIMIZATION
                         |
                         ▼
                 🔄 FIVE-FOLD CV
                         |
                         ▼
                 📊 EVALUATION
                         |
                         ▼
               🏆 MODEL COMPARISON
                         |
                         ▼
               🫀 RISK PREDICTION
```

The dataset was divided into 80% training and 20% testing data, with five-fold cross-validation used for model validation.

---

# 🧹 Data Preprocessing

Data preprocessing is an essential stage in developing reliable machine learning models.

The research examines several data preparation activities:

* Handling missing values.
* Identifying duplicate records.
* Examining inconsistent observations.
* Investigating potential outliers.
* Performing feature preparation.
* Applying feature selection.
* Preparing data for machine learning algorithms.

The objective is to improve data quality and establish a consistent foundation for model training and evaluation.

---

# ⚖️ Class Imbalance Handling

Class imbalance can affect the ability of machine learning models to identify minority-class observations.

This research incorporates two important approaches:

### 1. 🔵 Synthetic Minority Oversampling Technique (SMOTE)

SMOTE generates synthetic minority-class observations to improve class representation during model training.

### 2. 🟣 Class Weighting

Class weighting assigns different importance to classes during model training to help address classification bias.

### 📊 SMOTE Distribution

| Class                    | Original Distribution | After SMOTE |
| :----------------------- | --------------------: | ----------: |
| No Heart Attack Risk (0) |                 2,511 |       4,499 |
| Heart Attack Risk (1)    |                 2,511 |       4,499 |

**Important:** SMOTE is applied to training data rather than the held-out test data to avoid data leakage.

---

# 🤖 Machine Learning Models

The research compares seven supervised machine learning algorithms.

| No. | Algorithm                       | Category              |
| :-: | :------------------------------ | :-------------------- |
|  01 | 📈 Logistic Regression          | Linear Classification |
|  02 | 🌳 Decision Tree                | Tree-Based Learning   |
|  03 | 🌲 Random Forest                | Ensemble Learning     |
|  04 | 🚀 Gradient Boosting            | Boosting Algorithm    |
|  05 | ⚡ LightGBM                      | Gradient Boosting     |
|  06 | 🔥 AdaBoost                     | Adaptive Boosting     |
|  07 | 🧠 Multi-Layer Perceptron (MLP) | Neural Network        |

### 📈 Logistic Regression

A statistical classification algorithm used as a baseline for predicting binary outcomes.

### 🌳 Decision Tree

A tree-based learning algorithm that identifies patterns and relationships through decision rules.

### 🌲 Random Forest

An ensemble learning technique that combines multiple decision trees to improve prediction robustness.

### 🚀 Gradient Boosting

A boosting approach that sequentially develops models to improve predictive performance.

### ⚡ LightGBM

An efficient gradient-boosting framework designed for scalable tree-based learning.

### 🔥 AdaBoost

An adaptive boosting algorithm that focuses on observations incorrectly classified by previous learners.

### 🧠 Multi-Layer Perceptron (MLP)

A neural network architecture capable of learning complex nonlinear relationships in structured data.

---

# ⚙️ Hyperparameter Optimization

Hyperparameter optimization is incorporated to identify suitable configurations for the machine learning algorithms.

The process aims to improve model performance and establish more effective model configurations.

### Optimization Workflow

```text
       MACHINE LEARNING MODEL
                 |
                 ▼
       HYPERPARAMETER SEARCH
                 |
                 ▼
          MODEL VALIDATION
                 |
                 ▼
        FIVE-FOLD CROSS-VALIDATION
                 |
                 ▼
        OPTIMIZED CONFIGURATION
                 |
                 ▼
          FINAL EVALUATION
```

---

# 🔄 Five-Fold Cross-Validation

Five-fold cross-validation is used to assess model performance across different subsets of the training data.

```text
       FOLD 1 → TRAIN / VALIDATE
       FOLD 2 → TRAIN / VALIDATE
       FOLD 3 → TRAIN / VALIDATE
       FOLD 4 → TRAIN / VALIDATE
       FOLD 5 → TRAIN / VALIDATE
                    |
                    ▼
          AVERAGE PERFORMANCE
```

This approach provides a more comprehensive assessment of model performance than relying exclusively on a single validation split.

---

# 📊 Performance Evaluation Metrics

Healthcare prediction requires careful evaluation because identifying high-risk cases is particularly important.

The research incorporates multiple performance metrics.

| Metric               | Purpose                                              |
| :------------------- | :--------------------------------------------------- |
| 🎯 Accuracy          | Overall classification correctness                   |
| 🔎 Precision         | Correctness of positive predictions                  |
| ❤️ Recall            | Ability to identify actual positive cases            |
| ⚖️ F1-Score          | Balance between precision and recall                 |
| 📈 ROC-AUC           | Discrimination between positive and negative classes |
| 🧩 Confusion Matrix  | Detailed classification outcomes                     |
| 📊 Balanced Accuracy | Performance across both classes                      |

---

# 🏆 Key Findings

The experimental findings demonstrate that different algorithms perform differently depending on the evaluation criteria.

### 📊 Overall Model Comparison

| Machine Learning Model | Approx. Accuracy | Key Observation                    |
| :--------------------- | :--------------: | :--------------------------------- |
| 🌲 Random Forest       |        64%       | Strong overall classification      |
| 📈 Logistic Regression |        64%       | Competitive overall performance    |
| 🚀 Gradient Boosting   |        63%       | Strong ensemble performance        |
| ⚡ LightGBM             |        62%       | Competitive predictive performance |
| 🌳 Decision Tree       |        54%       | Better minority-class detection    |
| 🧠 MLP Neural Network  |        54%       | Better heart attack case detection |

*Values are approximate and based on the reported experimental results.*

### ❤️ Minority-Class Detection

An important finding is that the algorithm achieving the highest overall accuracy is not necessarily the most effective at identifying heart attack-risk cases.

The Decision Tree and MLP Neural Network demonstrated comparatively stronger minority-class detection through higher Recall and F1-Score.

### 🔥 Random Forest Performance

Random Forest achieved approximately:

| Metric    | Performance |
| :-------- | :---------: |
| Accuracy  |    64.3%    |
| Precision |    49.4%    |

### 📈 ROC-AUC Analysis

The reported ROC-AUC values were relatively close to random classification.

This indicates that the models demonstrated limited class-separation capability on the evaluated dataset.

### 💡 Important Research Observation

> Accuracy alone is insufficient for evaluating healthcare prediction models. Recall, Precision, F1-Score, and ROC-AUC provide additional insights into the ability of models to identify high-risk cases.

---

# 💡 Main Research Contributions

The primary contribution of this research is the development of a systematic comparative machine learning framework integrating:

* 🧹 Comprehensive data preprocessing.
* 🔍 Feature selection.
* ⚖️ Class imbalance handling.
* ⚙️ Hyperparameter optimization.
* 🔄 Five-fold cross-validation.
* 📊 Multi-metric performance evaluation.
* 🤖 Comparative analysis of seven machine learning algorithms.

The findings highlight the importance of evaluating machine learning models using multiple performance indicators rather than relying exclusively on accuracy.

---

# 🛠️ Technologies & Tools

| Technology          | Purpose                         |
| :------------------ | :------------------------------ |
| 🐍 Python           | Machine learning implementation |
| 📓 Jupyter Notebook | Experimental development        |
| 🐼 Pandas           | Data processing                 |
| 🔢 NumPy            | Numerical computation           |
| 🤖 Scikit-learn     | Machine learning algorithms     |
| ⚖️ Imbalanced-learn | SMOTE and class balancing       |
| 📊 Matplotlib       | Data visualization              |
| 🎨 Seaborn          | Statistical visualization       |
| 📈 Plotly           | Interactive visualization       |
| 📋 SPSS             | Statistical analysis            |

---

# 📂 Repository Structure

```text
A-Comparative-Machine-Learning-Framework/
│
├── 📄 A Comparative Machine Learning Framework for
│   Heart Attack Risk Prediction.docx
│
├── 📓 Data-Analysis-with-Python.ipynb
│
├── 📊 Heart_Attack_Risk_Levels_Dataset.csv
│
└── 📘 README.md
```

---

# 📚 Research Publication

The research manuscript is also available on **ResearchGate** for academic accessibility and research dissemination.

### 📖 Research Title

A Comparative Machine Learning Framework for Heart Attack Risk Prediction Using Data Preprocessing, Class Imbalance Handling, and Cross-Validation.

<div align="center">

<a href="https://www.researchgate.net/publication/408266268_A_Comparative_Machine_Learning_Framework_for_Heart_Attack_Risk_Prediction_Using_Data_Preprocessing_Class_Imbalance_Handling_and_Cross-Validation">

<img src="https://img.shields.io/badge/RESEARCHGATE-READ_FULL_RESEARCH-00CCBB?style=for-the-badge&logo=researchgate&logoColor=white" />
<a href="https://github.com/shahidazam2020-oss/A-Comparative-Machine-Learning-Framework-for-Heart-Attack-Risk-Prediction-Using-Data-Preprocessing">

<img src="https://img.shields.io/badge/GITHUB-EXPLORE_REPOSITORY-181717?style=for-the-badge&logo=github" />

</a>

</div>

---

# 🚀 Future Improvements

Potential directions for extending this research include:

* 🔬 External validation using independent healthcare datasets.
* 🧠 Integration of Explainable AI (XAI) techniques.
* 📊 SHAP-based feature importance analysis.
* ⚡ Advanced ensemble learning approaches.
* 🩺 Investigation of additional cardiovascular risk factors.
* 🔍 Advanced feature selection techniques.
* 📈 Model calibration and threshold optimization.
* 🌐 Development of an interactive prediction interface.

These are potential research extensions and are not claimed as completed implementations.

---

# 👨‍💻 Connect With Me

Thank you for exploring my research repository!

I am Shahid Azam, a Computer Science researcher specializing in Artificial Intelligence.

My academic and research interests include Machine Learning, Deep Learning, Artificial Intelligence, Natural Language Processing, Healthcare Analytics, and Intelligent Predictive Systems.

I welcome opportunities for academic collaboration, research discussions, and professional networking.

### 🌐 Professional & Academic Profiles

<div align="center">

<a href="https://github.com/shahidazam2020-oss">
<img src="https://img.shields.io/badge/GitHub-Follow_Me-181717?style=for-the-badge&logo=github" />
</a>

<a href="https://www.linkedin.com/in/shahid-azam-mughal-787b58235">
<img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin" />
</a>

<a href="https://www.researchgate.net/profile/Shahid-Azam-5">
<img src="https://img.shields.io/badge/ResearchGate-Explore_Research-00CCBB?style=for-the-badge&logo=researchgate" />
</a>

</div>

### 🔬 Research Interests

`Artificial Intelligence` · `Machine Learning` · `Deep Learning` · `Healthcare AI` · `Predictive Modeling` · `Explainable AI` · `Natural Language Processing` · `Large Language Models`

---

# 🤝 CONTRIBUTING

Contributions, suggestions, and constructive feedback are welcome!

This repository aims to support academic knowledge sharing and further research in machine learning and healthcare prediction.

### 🌟 How to Contribute

1. 🍴 Fork this repository.
2. 📥 Clone your fork.
3. 🌿 Create a new branch.
4. ✏️ Make your proposed improvements.
5. 📤 Submit a Pull Request.

### 💡 Contribution Areas

| Area                | Possible Contributions               |
| :------------------ | :----------------------------------- |
| 📚 Research         | Relevant academic publications       |
| 🤖 Machine Learning | Additional classification algorithms |
| ⚖️ Class Balancing  | Advanced imbalance-handling methods  |
| 🔍 Explainability   | SHAP and other XAI techniques        |
| 📊 Evaluation       | Additional performance metrics       |
| 📝 Documentation    | Corrections and improvements         |

<div align="center">

<a href="https://github.com/shahidazam2020-oss/A-Comparative-Machine-Learning-Framework-for-Heart-Attack-Risk-Prediction-Using-Data-Preprocessing/issues">

<img src="https://img.shields.io/badge/REPORT-Open_an_Issue-orange?style=for-the-badge&logo=github" />

</a>

<a href="https://github.com/shahidazam2020-oss/A-Comparative-Machine-Learning-Framework-for-Heart-Attack-Risk-Prediction-Using-Data-Preprocessing/pulls">

<img src="https://img.shields.io/badge/CONTRIBUTE-Pull_Request-success?style=for-the-badge&logo=github" />

</a>

</div>


---

<div align="center">

### 🫀 Machine Learning for Smarter Healthcare

**Data • Intelligence • Prediction • Research Innovation**

<br>

<sub>Research conducted by Shahid Azam and collaborators</sub>

<sub>© 2026 | Academic Research Project</sub>

</div>

---
## 🧪 Experimental Setup & Configuration

The experimental framework was designed to evaluate multiple machine learning algorithms under a consistent data preparation and validation strategy.

### ⚙️ Experimental Configuration

| Configuration           | Description                     |
| :---------------------- | :------------------------------ |
| 🎯 Learning Task        | Binary Classification           |
| 📊 Dataset              | Heart Attack Risk Prediction    |
| 🔀 Train-Test Split     | 80:20                           |
| 🔄 Cross-Validation     | 5-Fold                          |
| ⚖️ Imbalance Handling   | SMOTE and Class Weighting       |
| 🤖 Algorithms           | 7 Machine Learning Models       |
| 📈 Evaluation           | Multiple Classification Metrics |
| 🐍 Programming Language | Python                          |

### 🔬 Experimental Strategy

* Consistent preprocessing across model experiments.
* Training and testing data separation.
* Class imbalance handling within the training process.
* Hyperparameter optimization.
* Cross-validation-based performance assessment.
* Comparative evaluation of classification results.

> **Research Principle:** Fair model comparison requires consistent experimental conditions, appropriate validation, and reliable performance evaluation.

---
## 📊 Model Evaluation & Performance Analysis

Machine learning models are evaluated using multiple performance indicators to understand their classification capabilities.

### 📈 Evaluation Dimensions

| Evaluation Metric   | Research Importance                     |
| :------------------ | :-------------------------------------- |
| 🎯 Accuracy         | Overall predictive correctness          |
| 🔍 Precision        | Reliability of positive predictions     |
| ❤️ Recall           | Identification of actual positive cases |
| ⚖️ F1-Score         | Balance between Precision and Recall    |
| 📈 ROC-AUC          | Classification discrimination           |
| 🧩 Confusion Matrix | Classification error analysis           |

### 🏆 Performance Interpretation

The comparative analysis highlights an important distinction between overall classification accuracy and minority-class identification.

A model with higher accuracy does not necessarily provide better detection of heart attack-risk cases.

Therefore, Recall and F1-Score are particularly important when interpreting the predictive performance of healthcare classification models.

> **Key Insight:** Model selection should consider the intended application and the relative importance of false negatives and false positives, rather than accuracy alone.

---
## 🔁 Reproducibility & Research Transparency

Reproducibility is an important aspect of scientific machine learning research.

This repository provides supporting research materials to help readers understand the experimental methodology and research framework.

### 📚 Available Research Resources

| Resource                | Purpose                           |
| :---------------------- | :-------------------------------- |
| 📄 Research Manuscript  | Research methodology and findings |
| 📓 Jupyter Notebook     | Experimental implementation       |
| 📊 Dataset              | Supporting data for analysis      |
| 📘 README Documentation | Project overview and methodology  |

### 🔬 Research Transparency

The repository is intended to support:

* Understanding the experimental workflow.
* Reviewing the machine learning methodology.
* Examining the selected classification algorithms.
* Exploring preprocessing and class balancing strategies.
* Understanding model evaluation and reported findings.

> Reproducibility depends on using the same dataset version, preprocessing operations, feature configuration, random seeds, and model settings described in the research.

---
## 🧠 Research Limitations

Although this research investigates multiple machine learning approaches for heart attack risk prediction, several limitations should be considered.

### ⚠️ Identified Research Considerations

* **Dataset Dependency:** Experimental findings depend on the characteristics and quality of the selected dataset.
* **Generalizability:** Results may not directly generalize to different populations or healthcare environments.
* **Class Discrimination:** Relatively low ROC-AUC performance indicates limitations in distinguishing between the two classes.
* **Feature Dependency:** Predictive performance may depend on the availability and quality of input variables.
* **Clinical Validation:** The experimental framework has not established clinical effectiveness through independent real-world validation.

### 💡 Research Implications

These considerations highlight the need for independent datasets, improved feature engineering, advanced machine learning methods, explainability techniques, and clinical validation.

> **Research Perspective:** Machine learning predictions should be interpreted carefully, particularly in high-impact healthcare applications.

---
## 🔮 Research Impact & Academic Significance

This research contributes to the broader investigation of machine learning applications in healthcare risk prediction.

### 🌟 Academic Significance

* 📚 Provides a comparative investigation of seven machine learning algorithms.
* 🧹 Highlights the importance of systematic data preprocessing.
* ⚖️ Examines class imbalance handling in healthcare classification.
* 🔄 Incorporates cross-validation into model evaluation.
* 📊 Demonstrates the importance of multiple performance metrics.
* 🔬 Identifies opportunities for further research in healthcare AI.

### 🌍 Potential Research Applications

| Research Area              | Potential Contribution           |
| :------------------------- | :------------------------------- |
| 🏥 Healthcare AI           | Predictive modeling research     |
| 🫀 Cardiovascular Research | Risk classification studies      |
| 🤖 Machine Learning        | Comparative algorithm evaluation |
| 📊 Medical Data Science    | Data preprocessing and analysis  |
| 🔍 Explainable AI          | Interpretable predictive systems |

---
## 📚 How to Cite This Research

If you use, discuss, or reference this research in your academic work, please cite the original manuscript.

### 📖 Research Publication

**Title:** A Comparative Machine Learning Framework for Heart Attack Risk Prediction Using Data Preprocessing, Class Imbalance Handling, and Cross-Validation.

**Authors:** Shahid Azam and Dr. Adnan Amin.

**Year:** 2026.

### 🔗 Publication Access

<div align="center">

<a href="https://www.researchgate.net/publication/408266268_A_Comparative_Machine_Learning_Framework_for_Heart_Attack_Risk_Prediction_Using_Data_Preprocessing_Class_Imbalance_Handling_and_Cross-Validation">

<img src="https://img.shields.io/badge/ResearchGate-View_Publication-00CCBB?style=for-the-badge&logo=researchgate" />

</a>

</div>

### 📝 BibTeX Reference

```bibtex
@article{azam2026heartattack,
  title={A Comparative Machine Learning Framework for Heart Attack Risk Prediction Using Data Preprocessing, Class Imbalance Handling, and Cross-Validation},
  author={Azam, Shahid and Amin, Adnan},
  year={2026}
}
```

## *The BibTeX entry is a provisional citation template, not a verified journal publication record.*

---
## 🗺️ Research Roadmap

The following roadmap highlights potential directions for extending the current research framework.

### 🚀 Planned Research Directions

* [ ] 🔬 Validate models using independent healthcare datasets.
* [ ] 🧠 Integrate Explainable Artificial Intelligence (XAI).
* [ ] 📊 Apply SHAP for feature importance analysis.
* [ ] ⚡ Investigate advanced ensemble learning techniques.
* [ ] 🔍 Explore feature selection optimization.
* [ ] 🩺 Investigate additional cardiovascular risk indicators.
* [ ] 📈 Improve model calibration and threshold selection.
* [ ] 🌐 Develop an interactive research demonstration.

### 🎯 Long-Term Research Vision

Develop more reliable, interpretable, and generalizable machine learning approaches for healthcare risk prediction.

> These items represent potential future research activities, not completed project features.

---
# ⚠️ Important Research Disclaimer

This project is intended exclusively for academic, educational, and research purposes.

The machine learning models presented in this study are experimental predictive models and are not intended to replace professional medical diagnosis, clinical judgment, or validated clinical decision-support systems.

The reported results are specific to the dataset and experimental methodology used in this research. Independent clinical validation is necessary before considering any real-world healthcare application.

---

# 📜 License

This repository contains academic research materials, a research manuscript, dataset, and supporting notebook.

No formal license is currently specified for the research materials.

Please contact the author(s) for permission before redistributing or modifying the manuscript or other materials. Any third-party dataset remains subject to its original terms of use.

---
# ⭐ Support This Research

If you find this research useful for your academic studies, research activities, or professional interests:

* ⭐ Star this repository.
* 🔗 Share the research with your academic network.
* 📚 Read and explore the publication on ResearchGate.
* 💬 Provide constructive feedback and suggestions.

Your support and academic engagement are appreciated!

---
