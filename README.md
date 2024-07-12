# TASK-3
This task involves using the matplotlib library to visualize data.


import pandas as pd
import matplotlib.pyplot as plt

# Create a sample DataFrame
data = {
    'Month': ['January', 'February', 'March', 'April', 'May', 'June'],
    'Sales': [150, 200, 250, 300, 350, 400],
    'Expenses': [100, 150, 200, 250, 300, 350]
}
df = pd.DataFrame(data)

# Generate the bar chart
plt.figure(figsize=(10, 5))
plt.bar(df['Month'], df['Sales'], color='b', label='Sales')
plt.bar(df['Month'], df['Expenses'], color='r', alpha=0.5, label='Expenses')
plt.xlabel('Month')
plt.ylabel('Amount in USD')
plt.title('Monthly Sales and Expenses')
plt.legend()
plt.show()

# Generate the line chart
plt.figure(figsize=(10, 5))
plt.plot(df['Month'], df['Sales'], marker='o', color='b', label='Sales')
plt.plot(df['Month'], df['Expenses'], marker='s', color='r', label='Expenses')
plt.xlabel('Month')
plt.ylabel('Amount in USD')
plt.title('Monthly Sales and Expenses')
plt.legend()
plt.show()
