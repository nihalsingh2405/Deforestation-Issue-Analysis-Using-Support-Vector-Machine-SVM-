# Deforestation Issue Analysis Using Support Vector Machine (SVM)

## Project Overview
This educational machine-learning project demonstrates how a Support Vector Machine (SVM) classifier can classify sample environmental records into `YES` or `NO` deforestation categories using selected environmental and human-activity indicators.

**Important:** The included CSV is synthetically generated for learning and code testing. It is not real satellite, forestry, or field-survey data. Its labels are generated from an illustrative rule and must not be treated as verified deforestation observations or used for policy decisions.

## Dataset
File: `deforestation.csv`

The dataset contains 300 synthetic sample records with these columns:

| Column | Description |
|---|---|
| `FOREST_AREA_LOSS` | Illustrative forest-area-loss indicator (%) |
| `ANNUAL_RAINFALL` | Annual rainfall (mm) |
| `AVERAGE_TEMPERATURE` | Average temperature (°C) |
| `POPULATION_DENSITY` | Population density (people per km²) |
| `AGRICULTURAL_LAND` | Agricultural land indicator (%) |
| `LOGGING_ACTIVITY` | 0 = No, 1 = Yes |
| `WILDFIRE_INCIDENTS` | Illustrative number of wildfire incidents |
| `ROAD_CONSTRUCTION` | 0 = No, 1 = Yes |
| `DEFORESTATION` | Target label: `YES` or `NO` |

## Algorithm
- Support Vector Machine (SVM) with a linear kernel

## Tools and Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Project Workflow
1. Load the CSV dataset.
2. Separate input features and the target label.
3. Split the data into training and testing sets.
4. Standardize the input features.
5. Train the SVM classifier.
6. Predict the test-set labels.
7. Evaluate the model using accuracy, precision, recall, F1-score, and a confusion matrix.

## How to Run in Google Colab
1. Open a new notebook in Google Colab.
2. Upload `deforestation.csv` using the Files panel.
3. Install the libraries if needed:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
4. Run your Python code. Make sure it reads:
   ```python
   data = pd.read_csv("deforestation.csv")
   ```

## How to Run Locally
Place `deforestation.csv` and your Python script in the same folder, then run:
```bash
pip install -r requirements_deforestation.txt
python deforestation_analysis.py
```

## Disclaimer
This project is for educational demonstration only. The synthetic data and resulting model metrics do not represent real-world environmental measurements or validated deforestation predictions. For meaningful analysis, replace the sample CSV with a documented, real dataset and verify its target labels and feature definitions.
