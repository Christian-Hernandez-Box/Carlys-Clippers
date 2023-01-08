# Carlys-Clippers
You are the data analyst at Carly’s Clippers, the newest hair salon on the block. Your job is to go through the lists of data that have been collected in the past couple of weeks. You will be calculating some important metrics that Carly can use to plan out the operation of the business for the rest of the month.
```
# Carly's Clippers Data Points
hairstyles = ["bouffant", "pixie", "dreadlocks", "crew", "bowl", "bob", "mohawk", "flattop"]
prices = [30, 25, 40, 20, 20, 35, 50, 35]
last_week = [2, 3, 5, 8, 4, 4, 6, 2]

# Total Price of All Haircuts
total_price = 0
for price in prices:
  total_price += price
print("The total price of all haircuts is: $" + str(total_price))

# Average Haircut Price
average_price = total_price / len(prices)
print("The average haircut price is: $" + str(average_price))

# Reduce Haircut Prices by $5
new_prices = [low_price - 5 for low_price in prices]
print("The new haircuts prices are: " + str(new_prices))

# Calculating Revenue
total_revenue = 0

for i in range(len(hairstyles)):
  total_revenue += prices[i] * last_week[i]
print("Total revenue for last weeks haircuts were: $" + str(total_revenue))

# Average Daily Revenue
average_daily_revenue = total_revenue / len(prices)
print("The average daily revenue is $" + str(average_daily_revenue))

# Advertising Haircuts under $30
cuts_under_30 = [hairstyles[i] for i in range(len(hairstyles)) if new_prices[i] < 30]
print("The following haircuts are under $30 at Carly's Clippers. " + str(cuts_under_30) + " See you there!")
```
