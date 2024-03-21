# Data-Visualization-with-Pandas-and-Matplotlib


# Importing necessary libraries
import pandas as pd
import matplotlib.pyplot as plt

# Sample dataset (can be replaced with your own dataset)
data = {
    'Name': ['Alice', 'Bob', 'Charlie', 'David', 'Emma'],
    'Age': [25, 30, 35, 40, 45],
    'Salary': [50000, 60000, 70000, 80000, 90000]
}

# Creating a DataFrame from the dataset
df = pd.DataFrame(data)

# Displaying the DataFrame
print("DataFrame:")
print(df)
print()

# Summary statistics
print("Summary Statistics:")
print(df.describe())
print()

# Data visualization
plt.figure(figsize=(8, 5))
plt.bar(df['Name'], df['Salary'], color='skyblue')
plt.title('Salary Distribution')
plt.xlabel('Name')
plt.ylabel('Salary')
plt.show()
