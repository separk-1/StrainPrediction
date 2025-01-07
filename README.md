# StrainPrediction

A project for predicting strain in engineering systems using regression and time-series analysis.

## Project Structure
StrainPrediction/
├── README.md               # Project introduction and setup instructions
├── requirements.txt        # List of dependencies
├── run.py                  # Main script to run the project
├── data/                   # Directory to store datasets
└── .gitignore              # Git ignore file
```

## Setup Instructions

1. Clone the repository and navigate to the project directory:
   ```bash
   git clone <repository-url>
   cd StrainPrediction
   ```

2. Create and activate a Conda environment:
   ```bash
   conda create -n StrainPrediction python=3.11
   conda activate StrainPrediction
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Configure Jupyter Notebook to use the Conda environment:
   ```bash
   pip install ipykernel
   python -m ipykernel install --user --name=StrainPrediction --display-name "Python (StrainPrediction)"
   ```

5. Place the dataset (`StrainTemperature.csv`) in the `data/` directory.

6. Run the project using the Jupyter Notebook or main script:
   - To run the analysis in Jupyter Notebook:
     ```bash
     jupyter notebook run.ipynb
     ```
   - Or execute the main script:
     ```bash
     python run.py
     ```

## Requirements

Ensure the following dependencies are listed in `requirements.txt`:
```plaintext
numpy
pandas
scikit-learn
matplotlib
statsmodels
```

## Notes
- The `data/` folder should contain the dataset `StrainTemperature.csv`.
- The Conda environment must be activated before running the project.
