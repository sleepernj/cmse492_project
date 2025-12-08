# Predicting Diabetes Risk from Health Indicators

This project uses the *Diabetes Health Indicators Dataset* (originally collected by the U.S. Centers for Disease Control and Prevention through the Behavioral Risk Factor Surveillance System) to build machine learning models that predict whether an individual has diabetes based on demographic and lifestyle variables. The dataset contains over 200,000 survey responses and includes features such as Body Mass Index (BMI), physical activity, smoking status, age, and general health.  
The goal of this project is to use machine learning to identify the most important risk factors for diabetes and create a predictive model that can aid in early detection and prevention strategies.

---

## Repository Structure

```
cmse492_project/
├── README.md                <- Project overview and documentation
├── .gitignore               <- Files and folders ignored by Git
├── requirements.txt         <- Python dependencies for reproducibility
│
├── data/
│   ├── raw/                 <- Original dataset (diabetes_dataset.csv)
│   └── processed/           <- Processed data (e.g., diabetes_sample.csv)
│
├── notebooks/
│   └── final_project.ipynb  <- Final Jupyter notebook containing full analysis
│
├── figures/                 <- Visualizations generated from the notebook (ROC, SHAP, EDA)
│
├── reports/                 <- LaTeX project report, compiled PDF, project proposal
│   ├── Nick_Sleeper_CMSE492_FinalProject.tex
│   ├── Sleeper_Nick_CMSE492_FinalProject.pdf
│   └── Sleeper_Nick_CMSE492_ProjectProposal.pdf
│
└── structure.txt            <- Repository structure documentation
```

---

## Setup Instructions

**1. Clone the repository**

```bash
git clone https://github.com/sleepernj/cmse492_project.git
cd cmse492_project
```

**2. Install dependencies**

```bash
pip install -r requirements.txt
```

**3. Launch Jupyter Notebook**

```bash
jupyter notebook
```

Then navigate to `notebooks/exploratory/` to begin working with the dataset and initial analysis.

---

## Project Overview

- **Dataset:** Diabetes Health Indicators Dataset (Kaggle, derived from CDC BRFSS)  
- **Task Type:** Supervised Classification  
- **Goal:** Predict diabetes risk and identify key contributing health and lifestyle factors  
- **Planned Models:** Logistic Regression, Random Forest, Neural Network (MLPClassifier)  
- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-Score, ROC-AUC  

---

## Author

**Nick Sleeper**  
Michigan State University – CMSE 492 (Fall 2025)  
GitHub: [https://github.com/sleepernj](https://github.com/sleepernj)

## How to Run This Project

This section provides the full end-to-end instructions for reproducing the results, running the notebook, generating all figures, and compiling the LaTeX report. All steps below belong in a single markdown cell and can be copied and pasted directly.

---

### Step 1 — Clone the repository
```bash
git clone https://github.com/sleepernj/cmse492_project.git
cd cmse492_project
```

### Step 2 — (Optional but recommended) Create and activate a virtual environment
```bash
python3 -m venv venv
source venv/bin/activate        # macOS / Linux
venv\Scripts\activate           # Windows
```

### Step 3 — Install all required dependencies
```bash
pip install -r requirements.txt
```

### Step 4 — Launch Jupyter Notebook
```bash
jupyter notebook
```

Then open:

```
notebooks/final_project.ipynb
```

Running the notebook **top-to-bottom without interruption** will automatically:

- load and inspect the dataset  
- preprocess numeric and categorical features  
- split the data into train/validation/test sets  
- perform hyperparameter tuning using GridSearchCV  
- train Logistic Regression, Random Forest, and Gradient Boosting  
- evaluate all models on validation and test sets  
- generate ROC curves, SHAP plots, feature importance plots, and EDA plots  
- save all generated figures into `figures/`  
- export evaluation tables into `reports/`  

All figures referenced in the LaTeX report appear automatically in the `figures/` directory when the notebook is run.

---

### Step 5 — Recompile the LaTeX report (optional)
If you want to regenerate the final PDF after editing the `.tex` file:

```bash
cd reports
pdflatex Nick_Sleeper_CMSE492_FinalProject.tex
```

This produces:

```
Sleeper_Nick_CMSE492_FinalProject.pdf
```

---

### Step 6 — Output locations

- **Figures:** `figures/` (all EDA, ROC, SHAP, coefficient and importance plots)  
- **Notebook:** `notebooks/final_project.ipynb`  
- **LaTeX + PDF report:** `reports/`  
- **Processed sample data:** `data/processed/diabetes_sample.csv`  

---

### Step 7 — Hardware requirements

This project runs entirely on **CPU**. No GPU is required. Notebook execution takes only a few minutes on a standard laptop.

---

### Step 8 — Fully reproducing the results

To reproduce the project exactly:

1. Install dependencies  
2. Open the notebook  
3. Run every cell top-to-bottom  
4. (Optional) Rebuild the LaTeX report  
5. Confirm that figures appear in `figures/`  
6. Confirm CSV outputs appear in `reports/`  

