# Semiconductor Manufacturing Process – Pass/Fail Yield Prediction

This repository contains the capstone project notebook for predicting semiconductor pass/fail yield using sensor data from the SECOM dataset.

## Project Overview

The objective of this project is to build machine learning classification models to predict whether a semiconductor manufacturing observation will pass or fail based on process sensor measurements. The project includes:

- Data cleaning and preprocessing
- Missing value handling
- Duplicate and constant feature removal
- Class imbalance handling using SMOTE
- Model comparison and tuning
- Feature selection and threshold optimization
- Final model evaluation and saving

## Dataset

- Dataset: Semiconductor Manufacturing Process Sensor Data (SECOM)
- Shape: 1567 observations × 592 attributes
- Target variable: Pass/Fail
- Encoding:
  - -1 = Pass
  - 1 = Fail

Place the dataset file named `signal-data.csv` in the root folder of this repository before running the notebook.

## Repository Contents

- `Corizo_.ipynb` – full project notebook with analysis, preprocessing, modeling, and evaluation
- `README.md` – project overview and setup instructions
- `requirements.txt` – required Python dependencies
- `.gitignore` – standard project exclusions

## Environment Setup

1. Clone the repository.
2. Open a terminal in the project folder.
3. Create a virtual environment (optional but recommended):

   ```bash
   python -m venv .venv
   .venv\Scripts\activate
   ```

4. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

5. Open the notebook and run all cells in order.

## Dependencies

The project uses:

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- imbalanced-learn
- Joblib

## Notes

This project focuses on a highly imbalanced binary classification problem, so minority-class metrics such as recall, precision, and F1-score are emphasized alongside overall accuracy.

## Model Output

The notebook saves the final trained model as:

- `final_semiconductor_yield_model.pkl`

## License

This project is intended for educational and academic use.
