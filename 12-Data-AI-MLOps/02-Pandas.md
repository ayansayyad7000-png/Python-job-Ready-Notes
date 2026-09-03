# 02 — Pandas Basics

Install:
```bash
pip install pandas
```

## DataFrame
```python
import pandas as pd

df = pd.DataFrame({
    "server": ["api-1", "api-2"],
    "cpu": [45, 92],
})
```

## CSV
```python
df = pd.read_csv("metrics.csv")
df.to_csv("clean.csv", index=False)
```

## Inspect
```python
print(df.head())
print(df.info())
print(df.describe())
```

## Select / Filter
```python
print(df["cpu"])
critical = df[df["cpu"] >= 90]
```

## Missing Values
```python
df.isna().sum()
df = df.dropna()
# or
df["cpu"] = df["cpu"].fillna(0)
```

## Group
```python
summary = df.groupby("environment")["cpu"].mean()
```

## Company Use
ETL, reports, experiment/model data, analysis, batch pipelines.

## Practice
Load CSV → clean missing values → filter critical rows → save new CSV.
