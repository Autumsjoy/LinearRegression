# ACME Insurance: Health Premium Prediction

### Predicting Medical Charges using Linear Regression

This repository contains a machine learning project focused on predicting individual medical costs billed by health insurance for **ACME Insurance Company**. By leveraging customer demographics and health indicators, this model provides a data-driven approach to estimating annual premiums.

---

## 📌 Project Overview

The goal of this project is to build a predictive model that can accurately estimate the `charges` (medical costs) for a customer based on several independent variables. This helps ACME Insurance automate its pricing strategy and identify the most significant drivers of insurance costs.

### Key Features Used:

* **Age:** Age of primary beneficiary.
* **Sex:** Insurance contractor gender (female, male).
* **BMI:** Body mass index ($kg/m^2$).
* **Children:** Number of children/dependents covered.
* **Smoker:** Smoking status (yes, no).
* **Region:** The beneficiary's residential area in the US.

---

## 🚀 Getting Started

### Prerequisites

Ensure you have Python 3.8+ installed. You will need the following libraries:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn

```

### Installation

1. Clone the repository:
```bash
git clone https://github.com/your-username/acme-insurance-regression.git

```


2. Navigate to the project folder:
```bash
cd acme-insurance-regression

```


3. Run the model training script:
```bash
python model_training.py

```



---

## 📊 Model Performance

The model was built using **Multiple Linear Regression** with a standard 80-20 train-test split.

| Metric | Result |
| --- | --- |
| **Mean Absolute Error (MAE)** | $4,170.88 |
| **Mean Squared Error (MSE)** | $33,596,915.85 |
| **R-Squared ($R^2$) Score** | **0.75** |

> **Note:** Performance metrics are based on the baseline ACME dataset. Significant cost drivers identified include smoking status and BMI.

---

## 📂 Repository Structure

```text
├── data/
│   └── insurance.csv         # Raw dataset
├── notebooks/
│   └── exploratory_eda.ipynb # Data analysis and visualizations
├── src/
│   ├── preprocess.py        # Data cleaning and encoding
│   └── model_training.py    # Training the linear regression model
├── models/
│   └── acme_linear_reg.pkl  # Saved model artifact
└── README.md

```

---

## 📈 Key Findings

* **Smoking:** Smoker status is the highest weighted feature, contributing to a significant increase in predicted charges.
* **Age/BMI Interaction:** There is a clear linear correlation between age and cost, which is amplified as BMI increases.

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.
