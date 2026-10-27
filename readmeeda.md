# Titanic Dataset: Exploratory Data Analysis (EDA)

An exploratory data analysis of the Titanic passenger dataset, done in a Jupyter Notebook (`EDA.ipynb`) using Python, Pandas, Seaborn and Matplotlib. The goal is to understand the structure of the data, find missing values, and see which factors are related to passenger survival.

## Dataset

The dataset is loaded directly from Seaborn:

```python
titanic = sns.load_dataset('titanic')
```

- **Rows:** 891 passengers
- **Columns:** 15

| Column | Description |
|---|---|
| `survived` | Survival (0 = No, 1 = Yes) |
| `pclass` / `class` | Ticket class (1/2/3 or First/Second/Third) |
| `sex` | Gender |
| `age` | Age in years |
| `sibsp` | Number of siblings/spouses aboard |
| `parch` | Number of parents/children aboard |
| `fare` | Ticket fare |
| `embarked` / `embark_town` | Port of embarkation (C/Q/S) |
| `who` | man / woman / child |
| `adult_male` | Whether the passenger is an adult male |
| `deck` | Cabin deck |
| `alive` | Survival as yes/no |
| `alone` | Whether the passenger travelled alone |

## Requirements

- Python 3.x
- numpy
- pandas
- seaborn
- matplotlib
- jupyter

Install with:

```bash
pip install numpy pandas seaborn matplotlib jupyter
```

## How to Run

1. Clone or download this project.
2. Install the requirements above.
3. Start Jupyter:
   ```bash
   jupyter notebook EDA.ipynb
   ```
4. Run all cells from top to bottom.

## What the Notebook Covers

1. **Setup:** imports and loading the dataset
2. **Basic inspection:** `info()`, `head()`, `tail()`, `describe()`
3. **Target variable:** survival counts (`countplot`)
4. **Categorical features:** class, sex, `who` (pie chart) and embarkation town (bar chart)
5. **Subsetting:** passengers younger than 20
6. **Missing values:** `isnull().sum()` and a heatmap
7. **Distributions and relationships:** survival by sex and class, age histogram, age vs. fare scatter plots
8. **Correlation analysis:** correlation matrix and heatmap for numeric features

## Key Findings

- **Survival rate:** about 38.4% of passengers survived.
- **Missing data:**
  - `deck` is mostly missing (only 203 of 891 values present)
  - `age` has 177 missing values (714 present)
  - `embarked` / `embark_town` have 2 missing values
- **Age:** mean age is about 29.7 years, with a range from 0.42 to 80. 164 passengers were under 20.
- **Fare:** very skewed, with a mean of about 32.2 and a maximum of 512.33.
- **Correlation with survival:**

| Feature | Correlation with `survived` |
|---|---|
| `adult_male` | -0.557 |
| `pclass` | -0.338 |
| `fare` | +0.257 |
| `alone` | -0.203 |
| `parch` | +0.082 |
| `age` | -0.077 |
| `sibsp` | -0.035 |

Being an adult male and travelling in a lower class were the strongest negative factors for survival, while a higher fare (which goes with higher class) was positively related.

## Possible Next Steps

- Handle missing values (impute `age`, drop or engineer `deck`)
- Feature engineering (family size, title extraction)
- Build and evaluate a survival prediction model (e.g. Logistic Regression, Random Forest)

## Project Structure

```
.
├── EDA.ipynb       # Main analysis notebook
└── readmeeda.md    # This file
```
