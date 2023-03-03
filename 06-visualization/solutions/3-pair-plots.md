# Solution Hints for : 3 - pairplots

## House Sales

```python
data_location = '../data/house-sales-simplified.csv'
data_location = 'https://github.com/elephantscale/datasets/raw/master/house-prices/house-sales-simplified.csv'

house_sales = pd.read_csv(data_location)

sns.pairplot(house_sales)

```


---