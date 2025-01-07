
# 🌟 StrainPrediction

A project for predicting strain in engineering systems using regression and time-series analysis. This project focuses on addressing **multicollinearity issues** in linear regression models and predicting future strain values using current and past data.

---

## 📂 Project Structure
```plaintext
StrainPrediction/
├── README.md               # Project introduction and setup instructions
├── requirements.txt        # List of dependencies
├── run.ipynb               # Main script to run the project
├── data/                   # Directory to store datasets
└── .gitignore              # Git ignore file
```

---

## ⚙️ Setup Instructions

### 1. Clone the repository and navigate to the project directory:
```bash
git clone https://github.com/separk-1/StrainPrediction.git
cd StrainPrediction
```

### 2. Create and activate a Conda environment:
```bash
conda create -n StrainPrediction python=3.11
conda activate StrainPrediction
```

### 3. Install the required dependencies:
```bash
pip install -r requirements.txt
```

### 4. Configure Jupyter Notebook to use the Conda environment:
```bash
pip install ipykernel
python -m ipykernel install --user --name=StrainPrediction --display-name "Python (StrainPrediction)"
```

### 5. Place the dataset (`StrainTemperature.csv`) in the `data/` directory.

### 6. Run the project:
- **To analyze data with Jupyter Notebook**:
  ```bash
  jupyter notebook run.ipynb
  ```
- **Or execute the main script**:
  ```bash
  python run.py
  ```

---

## 📋 Requirements

The following dependencies are required and listed in `requirements.txt`:
- **numpy**: For numerical computations.
- **pandas**: For data manipulation and analysis.
- **scikit-learn**: For regression models and evaluation.
- **matplotlib**: For data visualization.
- **statsmodels**: For statistical modeling.

Install all dependencies using:
```bash
pip install -r requirements.txt
```

---

## 🎯 Project Objectives
1. **Calibrate Linear Regression Models**  
   Use the provided dataset (`StrainTemperature.csv`) to predict strain values based on six temperature measurements.
2. **Address Multicollinearity**  
   Investigate and solve multicollinearity issues using techniques like:
   - Subset Selection
   - Principal Component Analysis (PCA)
   - Ridge and Lasso Regression
3. **Future Strain Prediction**  
   Build models to predict strain 30 or 60 minutes into the future, using present and past data.

---

## 📌 Notes
- Ensure the `data/` folder contains the dataset `StrainTemperature.csv`.
- Activate the Conda environment before running the project.

---

## 👨‍🔬 About the Dataset
- The dataset contains **337 rows and 7 columns**:
  - Column 1: Strain measurements (in micro-strains, με).
  - Columns 2-7: Temperature measurements from six thermometers (in °C).
- Data is collected every **30 minutes for one week**.
