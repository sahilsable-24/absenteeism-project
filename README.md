
# 📊 Absenteeism Data Analysis Project

This project analyzes employee absenteeism to uncover key patterns and build a predictive machine learning model. It includes:

- Exploratory data analysis using Python
- A full ML pipeline to process new unseen data
- A Tableau dashboard for interactive insights
- Modular Python code for scalability

---

## 🎯 Project Goals

- Understand key causes of absenteeism using data
- Build a logistic regression model to predict risk
- Visualize insights using Tableau dashboards
- Provide reusable code to handle new prediction requests

---

## 🗂️ Repository Structure

```
absenteeism-project/
│
├── ABSENTEEISM_DATASET.ipynb       # EDA and basic logistic regression modeling
├── ABSENTTEEISM_ML.ipynb           # Complete ML pipeline using the module
├── absenteeism_module.py           # Python class to preprocess and predict new data
├── Absenteeism-data.csv            # Original dataset
├── Absenteeism_new_data.csv        # New data for predictions
├── Absenteeism_predictions.csv     # Prediction results from ML pipeline
├── df_preprocessed.csv             # Cleaned and processed dataset
├── Book1.twb                       # Tableau workbook for visual analysis
└── README.md                       # Project documentation (this file)
```

---

## 📊 Tableau Dashboard

- **File**: `Book1.twb`
- **Software**: Tableau Desktop
- **Dashboard Includes**:
  - Absenteeism trends by reason, month, department
  - Correlation between BMI and absence
  - Time-based trend analysis

> 💡 To view: Open in Tableau Desktop or Tableau Public.

---

## 🧠 Machine Learning Overview

### 🔹 absenteeism_module.py

Defines a custom `absenteeism_model` class that:

- Loads a saved logistic regression model and scaler
- Cleans and processes new input CSV data
- Predicts absenteeism risk (binary classification)
- Outputs prediction probability and result

Includes a `CustomScaler` class to standardize selected columns while preserving column order.

### 🔹 ABSENTEEISM_ML.ipynb

- Imports the custom module
- Loads `Absenteeism_new_data.csv`
- Cleans the data using the class method
- Generates predictions and saves them to `Absenteeism_predictions.csv`

---

## ⚙️ Technologies Used

- Python 3
- Pandas, NumPy
- Scikit-learn
- Jupyter Notebook
- Tableau Desktop
- Pickle (model serialization)

---

## ✅ How to Run the Project

1. **Clone this repository**:
   ```bash
   git clone https://github.com/sahilsable-24/absenteeism-project.git
   cd absenteeism-project
   ```

2. **Run notebooks**:
   - Start Jupyter Notebook
   - Open and run `ABSENTEEISM_ML.ipynb`

3. **Open Tableau dashboard**:
   - Launch `Book1.twb` using Tableau Desktop or Public

---

## 📈 Results

- Created a clean pipeline to prepare and model absenteeism data
- Built modular tools for applying the model to new unseen data
- Visualized results with clear, interactive dashboards

---

## 📌 Future Improvements

- Test other algorithms like Random Forest or XGBoost
- Deploy model via Flask/Django API for real-time use
- Improve dashboard interactivity with parameters and filters
- Integrate email alerts or reporting features

---

## 📬 Contact

For contributions, suggestions, or feedback:

- Open a GitHub Issue
- Submit a Pull Request
- Email: [sahilsable2407@gmail.com]
