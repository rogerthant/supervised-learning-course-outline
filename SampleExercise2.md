**Visualizing House Price Data**

You will now visualize the distribution of house prices and explore the relationship between house size and price.

You have a dataset `house_data` with columns 'price' (in thousands of dollars) and 'age' (in years). Your task is to create a histogram of house prices and a scatterplot of house size vs. price.

Matplotlib.pyplot has been imported as `plt`, and the dataset has been loaded for you.

**Instructions**
* Create a histogram of the 'price' column with 30 bins.
* Create a scatterplot with 'size' on the x-axis and 'price' on the y-axis.
* Add appropriate labels and titles to both plots.
* Display the plots.

```python
# Create a histogram of house prices
plt.figure(figsize=(12, 6))
plt.____(house_data['____'], ____=____)

# Label the x-axis and y-axis
plt.____('Price (thousands of dollars)') 
plt.____('Frequency')

# Set the title
____.____('Distribution of House Prices')

# Display the histogram
plt.____()

# Create a scatterplot of house size vs. price
plt.figure(figsize=(12, 6))
plt.____(____['____'], ____['____'])

# Label the x-axis and y-axis
plt.____('Size (square feet)')
plt.____('Price (thousands of dollars)')

# Set the title
plt.____('House Size vs. Price')

# Display the scatterplot
plt.____()
```
