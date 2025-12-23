# Mesterbakeren Sales Prediction

Sales prediction project using Prophet for time series forecasting.

## Project Structure

```
mesterbakeren/
├── colab/                    # Data files (Excel files)
│   ├── MB salg.xlsx         # Main sales data
│   ├── værtabell.xlsx       # Weather data
│   ├── produkter.xlsx       # Product data
│   ├── produktgruppe.xlsx   # Product group data
│   ├── salgbutikk1801.xlsx  # Store sales data
│   └── ferier.xlsx          # Holiday data
│
├── notebooks/                # Jupyter notebooks
│   └── Python_kode_for_Dataforberedelse_til_Prophet.ipynb
│
├── src/                      # Source code (for future refactoring)
│
└── README.md                 # This file
```

## Data Files

All data files (Excel files with `.xlsx` extension) are stored in the `colab/` folder. The notebook references these files using the `colab/` prefix in file paths.

## Notebook

The main analysis and modeling work is in the Jupyter notebook:
- `notebooks/Python_kode_for_Dataforberedelse_til_Prophet.ipynb`

This notebook contains:
- Data preparation functions
- Regressor creation (weekdays, weather, holidays)
- Prophet model training and prediction
- Visualization and evaluation functions
- Main execution script

## Usage

When running the notebook, ensure you are in the project root directory so that file paths like `colab/MB salg.xlsx` resolve correctly.
