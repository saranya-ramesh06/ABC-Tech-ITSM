# ITSM Incident Management with Machine Learning

**Client**: ABC Tech  
**Category**: ITSM - Machine Learning  

##  Project Description

A machine learning project to enhance IT service management at ABC Tech by predicting high-priority incidents, automating ticket tagging, and forecasting incident volumes for smarter resource planning.

##  Objectives

- Predict high-priority incidents to enable proactive issue resolution.
- Forecast incident volumes to support effective resource allocation.
- Automatically tag tickets with correct priority and department.
- Predict RFC failures to reduce service disruptions.

##  Data Overview

The dataset consists of incident management records with fields such as:

- **Incident_ID**: Unique ID of the incident  
- **CI_Name, CI_Cat, CI_Subcat**: Details about Configuration Items involved  
- **WBS**: Work Breakdown Structure information  
- **Status**: Current status of the ticket  
- **Priority, Department, Date Logged, Resolution Date**  
- (and other ITSM-relevant metadata)

Data was securely extracted from a SQL database and processed using Python.

##  Methodology

- **Data Preprocessing**: 
  - Cleaned nulls, outliers, and inconsistencies
  - Categorical encoding (Label Encoding, One-Hot Encoding)
  - Feature selection and dimensionality checks

- **Exploratory Data Analysis (EDA)**:
  - Trend analysis
  - High-priority ticket patterns
  - Incident distribution by CI and department

- **Machine Learning Models**:
  - Classification (e.g., Random Forest, Logistic Regression, XGBoost)
  - Regression (for volume forecasting)
  - Clustering (for auto-tagging and department assignment)

- **Class Imbalance Handling**: 
  - SMOTE applied for minority class oversampling

- **Model Evaluation Metrics**:
  - Accuracy, Precision, Recall, F1-Score, ROC-AUC

##  Key Visual Insights

- High attrition observed in Sales department  
- Work-life balance correlates with better performance  
- No direct correlation between pay and performance  
- High performers often receive salary hikes above 20%  
- Departments like Sales and R&D have the most incidents  

##  Outcomes

- Achieved 95% accuracy with RandomForestClassifier for performance prediction  
- Identified top features impacting performance and attrition  
- Provided actionable insights for improving ITSM strategy and operations  

##  Tools & Technologies

- Python (Pandas, NumPy, Scikit-learn, XGBoost, Seaborn, Matplotlib)  
- SQL (for data extraction)  
- Jupyter Notebook (for analysis and modeling)  
- SMOTE (for handling class imbalance)  

##  Data Security

- Data exported securely from SQL server  
- No sensitive credentials stored in code  
- All analysis was performed offline to maintain confidentiality  

##  Conclusion

This project successfully demonstrated the application of machine learning in ITSM for predictive incident management. By combining robust data preprocessing, insightful visualization, and high-performing ML models, ABC Tech can now better forecast incidents, reduce service disruptions, and automate routine ticketing tasks. These enhancements pave the way for a more efficient, proactive, and data-driven approach to IT operations.

