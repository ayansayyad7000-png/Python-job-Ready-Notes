# Pandas Basics

Pandas is used for tabular data processing.

Install:
```bash
python -m pip install pandas
```

```python
import pandas as pd

df = pd.read_csv("employees.csv")
print(df.head())
print(df.columns)
```

## Select and Filter
```python
active = df[df["active"] == True]
selected = df[["name", "salary"]]
```

## Missing Data
```python
print(df.isna().sum())
df["salary"] = df["salary"].fillna(0)
```

## Grouping
```python
summary = df.groupby("team")["salary"].mean()
```

## Company Use
Reports, ETL, data validation, ML datasets, analytics, experiment data.

## Common Mistakes
- Loading extremely large datasets without considering memory
- Chained assignment confusion
- Modifying raw data without keeping a reproducible pipeline

## Interview Questions
1. Series vs DataFrame?
2. What does `groupby()` do?