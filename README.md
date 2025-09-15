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




