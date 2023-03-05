# AirBNB Solution

## Info

```python
data.info()
```

## Describe

```python
data.describe()
```

## Neighborhood values

```python
data['neighbourhood_group'].value_counts()
```

## Correlation Matrix

```python
corr_matrix = data2.corr()
sns.heatmap(corr_matrix,   vmax=1, # xticklabels=corr.columns,  yticklabels=corr.columns,
            cmap='coolwarm', annot=True, annot_kws={'size': 10})
```