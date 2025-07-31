# Assignment

## Brief

Write the Python codes for the following questions.

## Instructions

Paste the answer as Python in the answer code section below each question.

### Question 1

Question: How do you create a 2x2 subplot grid in matplotlib and select the first subplot?

Answer:

```python
pip install matplotlib
import matplotlib.pyplot as plt

# Create a 2x2 grid of subplots
fig, axs = plt.subplots(2, 2)

# Select the first subplot (top-left)
ax1 = axs[0, 0]

# Now you can plot something on ax1
ax1.plot([1, 2, 3], [4, 5, 6])
ax1.set_title('First Subplot')

# Show the plot
plt.tight_layout()
plt.show()

```

### Question 2

Question: How to plot a line and set the color to red and style to dash in a matplotlib plot?

```python
x = [1, 2, 3, 4]
y = [1, 4, 9, 16]
```

Answer:

```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4]
y = [1, 4, 9, 16]

# Plot a red dashed line
plt.plot(x, y, color='red', linestyle='--')

plt.title("Red Dashed Line Plot")
plt.xlabel("X Axis")
plt.ylabel("Y Axis")
plt.grid(True)
plt.show()
```

### Question 3

Question: How to plot a histogram with 30 bins for `data` in matplotlib?

```python
data = np.random.randn(1000)
```

Answer:

```python
import matplotlib.pyplot as plt
import numpy as np

# Generate data
data = np.random.randn(1000)

# Plot the histogram with 30 bins
plt.hist(data, bins=30, color='skyblue', edgecolor='black')

plt.title("Histogram with 30 Bins")
plt.xlabel("Value")
plt.ylabel("Frequency")
plt.grid(True)
plt.show()
```

### Question 4

Question: How can you set the x-axis and y-axis labels in a matplotlib plot?

Answer:

```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4]
y = [1, 4, 9, 16]

plt.plot(x, y)

# Set axis labels
plt.xlabel("X Axis Label")
plt.ylabel("Y Axis Label")

plt.title("Labeled Plot")
plt.grid(True)
plt.show()
```

### Question 5

Question: How do you create a bar plot in seaborn using the `tips` dataset to show the average tip amount per day?

```python
import seaborn as sns
tips = sns.load_dataset('tips')
```

Answer:

```python
pip install seaborn
import seaborn as sns
import matplotlib.pyplot as plt

# Load the dataset
tips = sns.load_dataset('tips')

# Create the bar plot
sns.barplot(data=tips, x='day', y='tip', estimator='mean', palette='pastel')

# Add labels and title
plt.title("Average Tip Amount per Day")
plt.xlabel("Day of the Week")
plt.ylabel("Average Tip ($)")
plt.grid(True)
plt.show()
```

### Question 6

Question: How to create a box plot for total_bill categorized by day in the `tips` dataset using seaborn?

Answer:

```python
import seaborn as sns
import matplotlib.pyplot as plt

# Load the dataset
tips = sns.load_dataset('tips')

# Create the box plot
sns.boxplot(data=tips, x='day', y='total_bill', palette='Set2')

# Add a title and axis labels
plt.title("Distribution of Total Bill by Day")
plt.xlabel("Day of the Week")
plt.ylabel("Total Bill ($)")
plt.grid(True)
plt.show()
```

## Submission

- Submit the URL of the GitHub Repository that contains your work to NTU black board.
- Should you reference the work of your classmate(s) or online resources, give them credit by adding either the name of your classmate or URL.
