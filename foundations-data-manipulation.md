# Data Science Roadmap 2025 - Foundations: Data Manipulation

## Data Manipulation for Data Science

Data manipulation is a core skill in data science. It involves cleaning, transforming, and preparing data for analysis and modeling. 

### Essential Skills

*   **Data Cleaning:** Handling missing values, outliers, inconsistencies, and errors in data.
*   **Data Wrangling:** Transforming and structuring data into a usable format. This includes tasks like merging, joining, reshaping, and pivoting data.
*   **Exploratory Data Analysis (EDA):**  Techniques for visualizing and summarizing data to understand its characteristics, patterns, and relationships.
*   **Data Visualization:** Creating effective visualizations to communicate data insights.

### Code Snippets (Python)

#### Example: Data Cleaning with Pandas

```python
import pandas as pd
import numpy as np

# Sample DataFrame with missing values and duplicates
data = {'ID': [1, 2, 3, 4, 5, 5],
        'Value': [10, 20, np.nan, 40, 50, 50],
        'Category': ['A', 'B', 'A', 'C', 'B', 'B']}
df = pd.DataFrame(data)

# Handle missing values (fill with mean)
df['Value'].fillna(df['Value'].mean(), inplace=True)

# Remove duplicates
df.drop_duplicates(subset=['ID'], inplace=True)

print(df)
```

#### Example: Data Visualization with Seaborn

```python
import seaborn as sns
import matplotlib.pyplot as plt
import pandas as pd

# Sample DataFrame (assuming df is already created as in the previous snippet)

# Create a bar plot
sns.barplot(x='Category', y='Value', data=df)
plt.title('Bar Plot of Value by Category')
plt.show()
```

### Recommended Technologies

*   **Pandas:** Python library for data manipulation and analysis.
*   **NumPy:** Python library for numerical computing, essential for Pandas.
*   **SQL:**  Structured Query Language for database management and data manipulation.
*   **Data Visualization Libraries:** Matplotlib, Seaborn, Plotly for creating static, interactive, and dynamic visualizations.

### Resources

*   Online courses (e.g., DataCamp, Coursera, Udacity)
*   Pandas documentation (pandas.pydata.org/docs/)
*   "Python for Data Analysis" by Wes McKinney (covers Pandas extensively)
*   "Storytelling with Data" by Cole Nussbaumer Knaflic (for data visualization)

### Best Practices

*   Understand your data: data types, distributions, and potential issues.
*   Document your data cleaning and transformation steps.
*   Use visualization to explore and understand your data.
*   Follow data integrity principles to ensure data accuracy and reliability.
*   Learn SQL for efficient database interactions and data manipulation.

## Author - 3XCeptional