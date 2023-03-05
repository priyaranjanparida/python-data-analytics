# Explore house sales solution

## Describe

```python
house_prices.describe()

house_prices[["SalePrice"]].describe()
```

## Group by bedrooms

```python
bedroom_sales = house_prices.groupby("Bedrooms").size()
```

## Filter

```python
filtered2 = house_prices.loc  [ (house_prices['Bedrooms'] < 5) &
                                (house_prices['Bathrooms'] < 3)]
filtered2
```

## Correlation matrix

```python
house_prices.corr() 
```

## Find Most Expensive Zipcode

```python
house_prices['price_per_sqft'] = house_prices['SalePrice'] / house_prices['SqFtTotLiving']
zipcode_avg_price  = house_prices.groupby('ZipCode')['ZipCode', 'price_per_sqft'].mean()

```