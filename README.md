# Uber-Sales-Analytics
This comprehensive analysis contains detailed ride-sharing data from Uber operations for the year 2024, providing rich insights into booking patterns, vehicle performance, revenue streams, cancellation behaviors, and customer satisfaction metrics.

The goal of this analysis is to uncover insights from the data and make valuable recommendations for the company.

### Objectives of the Analysis
1. Data Importation.
2. Data exploration.
3. Data cleaning.
4. Booking patterns.
5. Customer ratings.
6. Distribution of vehicle types.


## Data and Library Importation

 ```python
# importing the necessary libraries
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import warnings
warnings.filterwarnings('ignore')
```

```python
# importing the dataset
df = pd.read_csv("/content/drive/MyDrive/Colab Notebooks/UBER ANALYTICS/ncr_ride_bookings.csv")
```

## Data Exploration
Before the commencement of the analysis, the data was examined by checking the shape of the data, the data types, and the missing values. The results of 
the exploration revealed that the dataset has about 150,000 rows, whereas certain fields like `Avg VTAT`	(10500), `Avg CTAT`	(48000), `Cancelled Rides by Customer`	(139500), `Reason for cancelling by Customer`	(139500), `Cancelled Rides by Driver`	(123000), `Driver Cancellation Reason`	(123000), `Incomplete Rides`	(141000), `Incomplete Rides Reason`	(141000), `Booking Value`	(48000), `Ride Distance`	(48000), `Driver Ratings`	(57000), `Customer Rating`	(57000), `Payment Method`	(48000) have missing entries.

## Summary Statistics








## Data Preprocessing
The data had to be adequately prepared before moving ahead with our analysis. Therefore, I
* Handled the missing values:
  
```python
# Dropping off data fields with so much missing values
df.drop(["Cancelled Rides by Customer","Reason for cancelling by Customer","Cancelled Rides by Driver","Driver Cancellation Reason","Incomplete Rides","Incomplete Rides Reason"],axis=1,inplace=True)
```



