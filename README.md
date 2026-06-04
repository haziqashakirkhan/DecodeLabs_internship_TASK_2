# DecodeLabs_internship_TASK_2
#  Titanic Survival Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange)
![Accuracy](https://img.shields.io/badge/Accuracy-79%25-success)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

##  Project Overview

This project predicts whether a passenger survived the Titanic disaster using Machine Learning techniques. The dataset was cleaned, analyzed, and processed before training a Random Forest Classifier.

The final model achieved **79% accuracy** on the test dataset.

---

##  Objective

The goal of this project is to build a classification model that can predict passenger survival based on various features such as age, gender, ticket class, fare, and family information.

---

## Dataset

The project uses the Titanic dataset containing passenger information.

### Features Used

- Pclass (Passenger Class)
- Sex
- Age
- SibSp (Siblings/Spouses Aboard)
- Parch (Parents/Children Aboard)
- Fare
- Embarked

### Target Variable

- Survived
  - 0 = Did Not Survive
  - 1 = Survived

---

##  Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook

---

##  Data Preprocessing

The following preprocessing steps were performed:

### Handling Missing Values

- Filled missing Age values using the median.
- Filled missing Embarked values using the most frequent value.

### Encoding Categorical Variables

- Sex:
  - Male → 0
  - Female → 1

- Embarked:
  - Converted into numerical features using One-Hot Encoding.

### Feature Selection

The following features were selected for model training:

- Pclass
- Sex
- Age
- SibSp
- Parch
- Fare
- Embarked

---

##  Exploratory Data Analysis (EDA)

Performed data visualization and analysis to identify important patterns and relationships.

### Analysis Included

- Survival distribution
- Gender-wise survival comparison
- Passenger class analysis
- Age distribution
- Fare distribution
- Correlation heatmap

---

##  Machine Learning Model

### Random Forest Classifier

The model was trained using:

```python
from sklearn.ensemble import RandomForestClassifier

model = RandomForestClassifier(
    n_estimators=100,
    random_state=42
)

model.fit(X_train, y_train)
```

---

##  Model Performance

| Metric | Score |
|----------|--------|
| Accuracy | 79% |

The Random Forest model performed well in predicting passenger survival and achieved an accuracy of **79%** on the test data.

---

##  Project Structure

```text
Titanic-Survival-Prediction/
│
├── Titanic_Survival_Prediction.ipynb
├── titanic.csv
├── README.md
└── requirements.txt
```

---

##  How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Titanic-Survival-Prediction.git
```

### 2. Navigate to the Project Folder

```bash
cd Titanic-Survival-Prediction
```

### 3. Install Required Libraries

```bash
pip install -r requirements.txt
```

### 4. Run Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
Titanic_Survival_Prediction.ipynb
```

---

##  Key Learnings

- Data Cleaning
- Missing Value Handling
- Feature Engineering
- Data Visualization
- Classification Models
- Random Forest Algorithm
- Model Evaluation
- Machine Learning Workflow

---

##  Future Improvements

- Hyperparameter Tuning
- Cross Validation
- Feature Selection Optimization
- XGBoost Implementation
- Streamlit Deployment

---

##  Author

**Haziqa Shakir**

Data Science Student | Machine Learning Enthusiast

---

###  If you like this project, don't forget to star the repository!
