# extract_orders.ipynb
Investments / Trading using robots / OrderBook  
Python script for data analysis, which helps identify successful entry points  
Snapshot from the order book for some investment instrument is taken as the data source  
The idea is to get the most popular positions and place an order there as well :)

```python
# I interested in four most right points on bids quantity axis
# it will be my possible positions in orders book

from matplotlib import pyplot as plt
orders.plot(kind='scatter', x='bids.quantity', y='bids.price', s=32, alpha=.8)
plt.gca().spines[['top', 'right']].set_visible(False)
plt.grid(True)
```
![image](bids_quantity.png)

## result .csv
|index|bids\.quantity|bids\.price|asks\.quantity|asks\.price|bids\.position|asks\.position|
|---|---|---|---|---|---|---|
|0|5339|10\.3|331947|10\.31|0|0|
|1|1043838|10\.29|491951|10\.32|30|20|
|2|466075|10\.28|1763654|10\.33|0|40|
|3|652009|10\.27|472709|10\.34|20|10|
|4|528438|10\.26|381369|10\.35|10|0|
|5|1854415|10\.25|392166|10\.36|40|0|
|6|442816|10\.24|494148|10\.37|0|30|
|7|291109|10\.23|444405|10\.38|0|0|
|8|292067|10\.22|275118|10\.39|0|0|
|9|351967|10\.21|324126|10\.4|0|0|
|10|415850|10\.2|336188|10\.41|0|0|
|11|255223|10\.19|470752|10\.42|0|0|
|12|275724|10\.18|313150|10\.43|0|0|
|13|254758|10\.17|224653|10\.44|0|0|
|14|64989|10\.16|155844|10\.45|0|0|
|15|195532|10\.15|185042|10\.46|0|0|
|16|72723|10\.14|89512|10\.47|0|0|
|17|92104|10\.13|234819|10\.48|0|0|
|18|107861|10\.12|227954|10\.49|0|0|
|19|88994|10\.11|150123|10\.5|0|0|


