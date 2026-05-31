# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
import matplotlib.pyplot as plt
import pandas as pd
from sklearn.datasets import load_iris

# STEP 1: Load dataset
iris = load_iris()

# STEP 2: Convert to DataFrame
df = pd.DataFrame(
   iris.data,
   columns=iris.feature_names
)
# STEP 3: Visualize data

# Line Plot
plt.figure(figsize=(6,4))
plt.plot(df["sepal length (cm)"])
plt.title("Line Plot")
plt.xlabel("Index")
plt.ylabel("Sepal Length")
plt.show()
```
<img width="447" height="327" alt="image" src="https://github.com/user-attachments/assets/19cad232-1358-41cf-94a5-be4fed64396b" />


```
# Histogram
plt.figure(figsize=(6,4))
plt.hist(df["petal length (cm)"], bins=10)
plt.title("Histogram")
plt.xlabel("Petal Length")
plt.ylabel("Frequency")
plt.show()
```
<img width="605" height="392" alt="image" src="https://github.com/user-attachments/assets/988bd88e-5259-42da-89de-2f63192bf649" />

```

# Scatter Plot
plt.figure(figsize=(6,4))
plt.scatter(
    df["sepal length (cm)"],
    df["petal length (cm)"]
)
plt.title("Scatter Plot")
plt.xlabel("Sepal Length")
plt.ylabel("Petal Length")
plt.show()
```
<img width="543" height="393" alt="image" src="https://github.com/user-attachments/assets/037f7ab9-f480-4f44-b3d3-76de8f8a7614" />

```

# Bar Plot
plt.figure(figsize=(6,4))
df.mean().plot(kind="bar")
plt.title("Average Feature Values")
plt.ylabel("Value")
plt.show()
```
<img width="573" height="483" alt="image" src="https://github.com/user-attachments/assets/5765e292-713c-42bd-8dda-3fd674789c58" />



```
# Box Plot
plt.figure(figsize=(6,4))
plt.boxplot(df["sepal width (cm)"])
plt.title("Box Plot")
plt.show()
```
<img width="534" height="376" alt="image" src="https://github.com/user-attachments/assets/18b7e238-5334-4df9-8546-0bffc8f00c77" />


# Result:
The program was executed and verified succesfully.
