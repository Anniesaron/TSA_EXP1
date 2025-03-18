# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```
import pandas as pd
import matplotlib.pyplot as plt


file_path = "/content/weather_classification_data.csv"  # Replace with your actual file path
data = pd.read_csv(file_path)


data.index = pd.date_range(start="2025-01-01", periods=len(data), freq="D")


plt.figure(figsize=(10, 6))
plt.plot(data.index, data["Temperature"], label="Temperature", color="blue")


plt.title("Temperature Over Time")
plt.xlabel("Date")
plt.ylabel("Temperature (°C)")
plt.grid(True)
plt.legend()


plt.show()

```








# OUTPUT:





![Screenshot 2025-03-17 182851](https://github.com/user-attachments/assets/1f79e0b8-a5f2-45df-8fc5-d126bbd828bb)



# RESULT:
Thus we have created the python code for plotting the time series of given data.
