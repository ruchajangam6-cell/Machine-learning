# Data Preprocessing Experiment

A Jupyter notebook workspace for preparing data before analysis or modelling.

## Project Structure

```
.
├── data_preprocessing.ipynb   # Main experiment notebook
└── README.md                  # This file
```

## Environment

| Item        | Details                          |
|-------------|----------------------------------|
| Language    | Python 3.13.9                    |
| Environment | Conda (`base`)                   |
| Interface   | Jupyter Notebook / JupyterLab    |

## Getting Started

1. Install [Anaconda](https://www.anaconda.com/) or Miniconda.
2. Clone or download this project.
3. Launch Jupyter from the project folder:
   ```bash
   jupyter notebook
   ```
4. Open `data_preprocessing.ipynb` and run the cells in order (**Kernel → Restart & Run All**).

## Current Status

The notebook currently contains a setup check cell (`print("Hello World!")`) confirming the kernel runs correctly. The preprocessing steps below are still to be implemented.

## Planned Workflow

1. **Load data**: read the raw dataset (CSV, Excel, etc.) into a DataFrame.
2. **Inspect data**: check shape, data types, summary statistics and sample rows.
3. **Handle missing values**: drop or impute (mean / median / mode).
4. **Remove duplicates and outliers**.
5. **Encode categorical variables**: label or one-hot encoding.
6. **Scale / normalize features**: standardization or min-max scaling.
7. **Split data**: train and test sets.
8. **Save processed data** for downstream use.

## Suggested Libraries

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

## Results

_To be added once preprocessing is complete (e.g. cleaned dataset shape, summary of changes, plots)._

## Author

_Add your name here._

## License

_Add a license if you plan to share this project._
