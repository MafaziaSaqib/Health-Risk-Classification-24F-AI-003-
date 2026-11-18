# 🩺 Health Risk Classification – Diabetes Prediction

A Machine Learning project developed as part of an open-ended lab assessment for the Machine Learning course.

This project explores the use of classification algorithms to predict whether a patient is likely to have diabetes based on medical and health-related attributes. It uses the Pima Indians Diabetes Dataset and compares two machine learning models: Support Vector Machine (SVM) and Decision Tree.

## 📌 Project Overview

The objective of this project is to apply fundamental Machine Learning concepts to a healthcare-related classification problem.

The dataset contains patient information such as glucose level, blood pressure, BMI, age, insulin, and other medical attributes. Using these features, the models classify patients into two categories:

- **0 – No Diabetes**
- **1 – Diabetes**

## 📂 Dataset

**Pima Indians Diabetes Dataset**

- Source: [Pima Indians Diabetes Dataset](https://raw.githubusercontent.com/jbrownlee/Datasets/master/pima-indians-diabetes.data.csv)
- Total Records: 768
- Input Features: 8
- Target Variable: Outcome

### Features Used

| Feature | Description |
|---|---|
| Pregnancies | Number of pregnancies |
| Glucose | Plasma glucose concentration |
| BloodPressure | Diastolic blood pressure |
| SkinThickness | Triceps skinfold thickness |
| Insulin | Two-hour serum insulin |
| BMI | Body Mass Index |
| DiabetesPedigree | Diabetes pedigree function |
| Age | Patient's age |
| Outcome | Diabetes classification (0 or 1) |

## ⚙️ Technologies & Libraries

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## 🔬 Methodology

The project follows these Machine Learning steps:

**1. Data Loading**
- Imported the dataset using Pandas.
- Assigned appropriate column names.

**2. Data Preprocessing**
- Identified zero values in selected medical attributes.
- Replaced invalid zero values with missing values (`NaN`).
- Handled missing values using median imputation.

**3. Train-Test Splitting**
- Separated input features (X) and target variable (y).
- Split the dataset into 80% training and 20% testing data.

**4. Feature Scaling**
- Applied StandardScaler to standardize numerical features.
- Fitted the scaler on training data and transformed both training and testing data.

**5. Model Training**
Trained two classification algorithms:
- Support Vector Machine (SVM)
- Decision Tree Classifier

**6. Model Evaluation**
- Calculated model accuracy.
- Generated confusion matrices.
- Compared the performance of both classifiers.

## 🤖 Machine Learning Models & Results

The following results were obtained using the test dataset:

| Algorithm | Accuracy |
|---|---:|
| Support Vector Machine (SVM) | 74.68% |
| Decision Tree | 71.43% |

**Best Performing Model: Support Vector Machine (SVM)**

SVM achieved higher accuracy than the Decision Tree model on the test dataset.

## 📊 Evaluation Techniques

- Accuracy Score
- Confusion Matrix
- Classification Report (imported for evaluation)

Confusion matrices were generated to examine the correct and incorrect predictions made by each model.

## ▶️ How to Run the Project

**Requirements:**
- Python installed
- Jupyter Notebook
- Required Python libraries

**Step 1: Clone the repository**

```bash
git clone YOUR_REPOSITORY_URL
```

**Step 2: Navigate to the project folder**

```bash
cd Health-Risk-Classification
```

**Step 3: Install dependencies**

```bash
pip install pandas numpy matplotlib scikit-learn notebook
```

**Step 4: Launch Jupyter Notebook**

```bash
jupyter notebook
```

**Step 5:** Open the `Health Risk Classification.ipynb` notebook and run the cells sequentially.

## 📚 Learning Outcomes

Through this project, I gained practical experience with:

- Handling missing and invalid dataset values.
- Performing data preprocessing and feature scaling.
- Splitting datasets into training and testing sets.
- Implementing classification algorithms using Scikit-learn.
- Evaluating models using accuracy and confusion matrices.
- Comparing the performance of different ML algorithms.

## ⚠️ Disclaimer

This project is developed for educational purposes only. Its predictions are not intended for medical diagnosis or clinical decision-making.

---

**Developed by:** Mafazia Saqib  
**Course:** Machine Learning – Open-Ended Lab Project  
**Program:** BS Artificial Intelligence
