
# 👩‍💼 HR Analytics - Employee Attrition Prediction

This project focuses on building machine learning models to predict employee attrition based on various HR features. The goal is to help organizations proactively identify employees who are likely to leave and take preventive actions.

## 📁 Project Structure

```
HR_Analytics_Attrition/
│
├── HR analytics.ipynb        # Main Jupyter notebook with full analysis
├── README.md                 # Project documentation (this file)
└── models/                   # (Optional) Folder to store serialized models
```

## 📊 Dataset Description

The dataset includes features such as:

- **Attrition**: Target variable indicating whether the employee left the company
- **MonthlyIncome**, **HourlyRate**, **JobSatisfaction**, **OverTime**
- **Age**, **Gender**, **Department**, **JobRole**, **TotalWorkingYears**
- **YearsAtCompany**, **YearsInCurrentRole**, **YearsSinceLastPromotion**
- ...and many other HR-related factors

## ⚙️ Technologies Used

- Python 🐍
- Pandas, NumPy (data handling)
- Seaborn, Matplotlib (visualization)
- Scikit-learn (modeling)
- RandomForestClassifier, Logistic Regression, etc.

## 🧪 Project Workflow

1. **Data Preprocessing**
   - Encoding categorical variables
   - Handling missing values
   - Removing outliers
   - Feature selection and engineering

2. **Exploratory Data Analysis (EDA)**
   - Distribution of attrition across departments, roles, income levels
   - Correlation heatmaps
   - Boxplots, histograms, countplots

3. **Model Building**
   - Logistic Regression
   - Random Forest Classifier
   - Performance metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC

4. **Best Model**
   - **Random Forest Classifier** gave the best results using:
     ```
     n_estimators=10, max_depth=3, max_features='sqrt', min_samples_split=10
     ```

## 📈 Model Evaluation

| Model                  | Accuracy | F1-Score | ROC-AUC |
|-----------------------|----------|----------|---------|
| Random Forest          | 0.84     | 0.70     | 0.88    |
| Logistic Regression    | ...      | ...      | ...     |

(*Replace `...` with actual values from your notebook.*)

## 💡 Key Insights

- **OverTime**, **MonthlyIncome**, and **StockOptionLevel** are strong predictors of attrition.
- Long tenure without promotion increases the likelihood of attrition.
- Feature importance helps in HR decision-making.

## 🚀 Future Enhancements

- Hyperparameter tuning with GridSearchCV
- Create a Streamlit web app for user-friendly predictions
- Deploy model using Flask or FastAPI for REST API access

## 📌 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/hr-analytics-attrition.git
   cd hr-analytics-attrition
   ```

2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch the Jupyter Notebook:
   ```bash
   jupyter notebook "HR analytics.ipynb"
   ```
