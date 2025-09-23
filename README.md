# 2025-Y2-S1-MLB-B6G1-05-PGNO-105
IT2011 Group Project: Heart Disease Risk Prediction

## Overview
This project aims to design, implement, and evaluate an end-to-end AI/ML solution to predict heart disease risk using supervised learning techniques. The focus is on a real-world healthcare problem, leveraging a synthetic dataset to identify high-risk patients based on symptoms, lifestyle, and medical features. The solution will include data preprocessing, exploratory data analysis (EDA), model training, and a critical evaluation of performance and ethical implications, aimed at healthcare providers for early intervention.
## Dataset Details
- **Source**: Kaggle - Heart Disease Risk Prediction Dataset
- **Link**: [https://www.kaggle.com/datasets/mahatiratusher/heart-disease-risk-prediction-dataset](https://www.kaggle.com/datasets/mahatiratusher/heart-disease-risk-prediction-dataset)
- **Size**: Approximately 70,000 records
- **Type**: Tabular (Structured)
- **Features**: ~17 features (e.g., Age, Sex, ChestPain, Cholesterol, Smoking, Obesity, BloodPressure, Glucose, BMI, ShortnessOfBreath) excluding the target variable `Heart_Risk` (binary: 0 = Low Risk, 1 = High Risk)
- **Justification**: The dataset meets the minimum requirement of ≥6 features and ≥1,000 records. Its large size and synthetic nature ensure robustness for ML modeling, while the variety of features (demographic, lifestyle, medical) aligns with the healthcare domain for predicting heart disease risk. Data is clean (no missing values per Kaggle), enhancing feasibility.
- **Alternatives Considered**: UCI Heart Disease (303 records, rejected for size); Framingham Heart Study (narrow focus on cholesterol, less comprehensive).
## Group Member Roles
- IT24101185 (Member 1 - [Ranasinghe R.M.D.V]): Handling Missing Data & Dimension Reduction
- IT24101256 (Member 2 - [Niruba.N]): Encoding Categorical Variables
- IT24101128 (Member 3 - [Jayathungage D.K.C]): Outlier Removal
- IT24101086 (Member 4 - [Weerasinghe W.A.T.V]): Normalization/Scaling
- IT24101236 (Member 5 - [Rajapaksha R.A.J.K]): Feature Engineering
- IT24101205 (Member 6 - [Mahalonage C.A.S]): Feature Selection 

## How to Run the Code
1. **Prerequisites**: Ensure Python 3.x is installed with the following libraries:
   - `pip install pandas scikit-learn seaborn matplotlib jupyter`
2. **Steps**:
   - Navigate to the `Group_ID/` directory in your terminal.
   - Launch Jupyter Notebook: `jupyter notebook`
   - Open individual notebooks (e.g., `IT24101185_Handling_Missing.ipynb`) or `group_pipeline.ipynb` from the `notebooks/` folder.
   - Run cells sequentially to execute preprocessing techniques and view EDA visualizations.
3. **Dataset Location**: Ensure `heart_disease_risk.csv` is placed in the `data/raw/` subdirectory.
   - Note: Ensure all notebooks are in the `notebooks/` folder before running.
## Additional Notes
- **Progress Review I**: This repo contains notebooks for viva demo, integrating all preprocessing steps into `group_pipeline.ipynb`.
- **Ethical Considerations**: Synthetic data avoids privacy issues but may lack real-world bias representation, which will be explored in the evaluation stage.
- **Collaboration**: Repo tracked on GitHub for version control and teamwork evidence (pending setup).
## Repository Structure
Group_ID/
├── README.md
├── data/
│   └── raw/heart_disease_risk.csv
├── notebooks/
│   ├── IT24101185_Handling_Missing.ipynb
│   ├── IT24101256_Encoding_Categoricals.ipynb
│   ├── IT24101128_Outlier_Removal.ipynb
│   ├── IT24101086_Normalization_Scaling.ipynb
│   ├── IT24101236_Feature_Engineering.ipynb
│   ├── IT24101205_Feature_Selection_PCA.ipynb
│   └── group_pipeline.ipynb
└── results/
    ├── eda_visualizations/
    ├── logs/
    └── outputs/
## Preprocessing Pipeline
Raw Dataset
   ↓
1. Handling Missing Data → Member 1
   ↓
2. Encoding Categorical Variables → Member 2
   ↓
3. Outlier Removal → Member 3
   ↓
4. Normalization / Scaling → Member 4
   ↓
5. Feature Engineering → Member 5
   ↓
6. Feature Selection / PCA → Member 6
   ↓
Final Processed Dataset → results/outputs/final_processed.csv

---
*Last Updated: September 23, 2025*
