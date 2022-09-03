# ACM Research Coding Challenge (Fall 2022) - CarsForSale

## Problem
I attempted to sort each car trait based on how they affected the price. String-type variable columns besides the 'Price' column were not included, as I could not properly sort them.

## Solution
I first imported the data using a Kaggle notebook. Using a pandas Dataframe made from the csv, I converted the 'Price' column from string to int. Then, I separated the 'Price' column from the Dataframe and removed any 'Not Priced' variables, replacing them with the average of the prices. Using each column of the matrix as *x* values and the prices as *y* values, I performed linear regression to see which one affected the price. The ouput is here below:

```
Most influential factors on price:
#  1 :	 MaxMPG               	 0.1200
#  2 :	 ConsumerRating       	 0.0933
#  3 :	 PerformanceRating    	 0.0636
#  4 :	 ExteriorStylingRating 	 0.0305
#  5 :	 Year                 	 0.0115
#  6 :	 SellerReviews        	 0.0086
#  7 :	 ComfortRating        	 0.0050
#  8 :	 ReliabilityRating    	 0.0029
#  9 :	 ConsumerReviews      	 0.0016
# 10 :	 InteriorDesignRating 	 0.0013
# 11 :	 SellerRating         	 0.0004
# 12 :	 ValueForMoneyRating  	 0.0001
# 13 :	 MinMPG               	 0.0000
```

According to my solution, none of these variables seem to correlate with price.
