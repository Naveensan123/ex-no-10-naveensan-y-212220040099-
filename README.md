# ex-no-10-naveensan-y-212220040099-
# AIM
To Perform Data Visualization on a complex dataset and save the data to a file.

# EXPLANATION
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# ALGORITHM
# STEP 1 
Read the given Data 
# STEP 2 
Clean the Data Set using Data Cleaning Process 
# STEP 3 
Apply Feature generation and selection techniques to all the features of the data set 
# STEP 4 
Apply data visualization techniques to identify the patterns of the data.

# CODE
/* Data Visualization - Iris.csv

import pandas as pd

import seaborn as sns

import matplotlib.pyplot as plt

df = pd.read_csv("/content/iris.csv")

df.head()

df.info()

df["variety"].value_counts()

sns.countplot(x='variety', data=df, )

plt.show()

sns.scatterplot(x='sepal.length', y='sepal.width', hue='variety', data=df, )

plt.legend(bbox_to_anchor=(1, 1), loc=2)

plt.show()

sns.scatterplot(x='petal.length', y='petal.width', hue='variety', data=df, )

plt.legend(bbox_to_anchor=(1, 1), loc=2)

plt.show()

sns.pairplot(df.drop(['Id'], axis = 1), hue='variety', height=2)

fig, axes = plt.subplots(2, 2, figsize=(10,10))

axes[0,0].set_title("Sepal Length")

axes[0,0].hist(df['sepal.length'], bins=7)

axes[0,1].set_title("Sepal Width")

axes[0,1].hist(df['sepal.width'], bins=5);

axes[1,0].set_title("Petal Length")

axes[1,0].hist(df['petal.length'], bins=6);

axes[1,1].set_title("Petal Width")

axes[1,1].hist(df['petal.width'], bins=6);

sns.heatmap(df.corr(method='pearson').drop(['Id'], axis=1).drop(['Id'], axis=0), annot = True);

plt.show()

# OUTPUT

# RESULT
Thus the Data Visualization![download](https://github.com/Naveensan123/ex-no-10-naveensan-y-212220040099-/assets/95761973/4e79b27d-52df-4a5a-af89-d3b76b0a155a)
 for the given dataset had been executed successfully.
