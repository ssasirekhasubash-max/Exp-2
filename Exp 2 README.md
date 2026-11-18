# Experiment 2: Data Visualization Using Matplotlib and Seaborn

## Aim

To visualize data using Matplotlib and Seaborn libraries.

## Algorithm

1.  **Start.**
2.  Import the Matplotlib and Seaborn libraries.
3.  Load data into a Pandas DataFrame.
4.  Plot a histogram for age distribution using `plt.hist()`.
5.  Plot a scatter plot for Age vs. Salary using `sns.scatterplot()`.
6.  Plot salary distribution using `sns.boxplot()`.
7.  Show the plots sequentially.
8.  **Stop.**


## Program
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Create dataset
data = {
    'Age': [22, 25, 28, 30, 32, 35, 38, 40, 42, 45],
    'Salary': [18000, 22000, 25000, 30000, 35000,
               40000, 45000, 50000, 55000, 60000]
}

df = pd.DataFrame(data)

# Histogram
plt.hist(df['Age'], bins=5, edgecolor='black')
plt.title('Age Distribution')
plt.xlabel('Age')
plt.ylabel('Frequency')
plt.show()

# Scatter Plot
sns.scatterplot(x='Age', y='Salary', data=df)
plt.title('Age vs Salary')
plt.show()

# Box Plot
sns.boxplot(y=df['Salary'])
plt.title('Salary Distribution')
plt.show()

## output
Histogram – Age Distribution
 <img width="690" height="440" alt="image" src="https://github.com/user-attachments/assets/ddd5e343-d3f3-4d57-b173-2081fc33594d" />
 
 Scatter Plot – Age vs Salary
<img width="689" height="440" alt="image" src="https://github.com/user-attachments/assets/730f2a69-9a50-4885-bf28-a28543160255" />

Box Plot – Salary Distribution

<img width="690" height="440" alt="image" src="https://github.com/user-attachments/assets/66eded9c-08e3-4f3f-bce0-20639d75e86d" />


## result

Thus, data visualization was successfully performed using Matplotlib and Seaborn libraries. Histogram, scatter plot and box plot were created to analyse employee age and salary distribution.
