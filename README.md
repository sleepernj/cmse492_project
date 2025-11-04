# cmse492_project
# Predicting Diabetes Risk from Health Indicators

This project uses the *Diabetes Health Indicators Dataset* (originally collected by the U.S. Centers for Disease Control and Prevention through the Behavioral Risk Factor Surveillance System) to build machine learning models that predict whether an individual has diabetes based on demographic and lifestyle variables. The dataset contains over 200,000 survey responses and includes features such as Body Mass Index (BMI), physical activity, smoking status, age, and general health.  
The goal of this project is to use machine learning to identify the most important risk factors for diabetes and create a predictive model that can aid in early detection and prevention strategies.

---

## 📁 Repository Structure
cmse492_project/
├── README.md                <- Project overview and documentation
├── .gitignore               <- Files and folders ignored by Git
├── requirements.txt          <- Python dependencies for reproducibility
│
├── data/
│   ├── raw/                  <- Original data files (unmodified)
│   └── processed/            <- Cleaned and preprocessed data ready for modeling
│
├── notebooks/
│   └── exploratory/          <- Jupyter notebooks for exploratory data analysis (EDA)
│
├── src/
│   ├── preprocessing/        <- Data cleaning and feature engineering scripts
│   ├── models/               <- Machine learning model definitions and training scripts
│   └── evaluation/           <- Model evaluation and metrics scripts
│
├── figures/                  <- Visualizations generated from notebooks and scripts
└── docs/                     <- Reports, LaTeX proposal, and documentation files

---

---

## ⚙️ Setup Instructions  
  1. Clone the repository
git clone https://github.com/sleepernj/cmse492_project.git
cd cmse492_project
	2.	Install dependencies
pip install -r requirements.txt
  3. Launch Jupyter Notebook
jupyter notebook
Navigate to notebooks/exploratory/ to begin working with the dataset and initial analysis.

Project Overview
	•	Dataset: Diabetes Health Indicators Dataset (Kaggle, derived from CDC BRFSS)
	•	Task Type: Supervised Classification
	•	Goal: Predict diabetes risk and identify key contributing health and lifestyle factors
	•	Planned Models: Logistic Regression, Random Forest, and Neural Network (MLPClassifier)
	•	Evaluation Metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC

  Author

Nick Sleeper
Michigan State University – CMSE 492 (Fall 2025)
GitHub: https://github.com/sleepernj
