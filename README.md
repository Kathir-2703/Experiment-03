# Experiment-03-Univariate-Analysis

# AIM

To read the given data and perform Univariate Analysis.

# Explanation

Univariate analysis explores each variable in a data set, separately. It looks at the range of values, as well as the central tendency of the values. It describes the pattern of response to the variable. It describes each variable on its own.

# ALGORITHM

# STEP 1

Read the given Data

# STEP 2

Get the information about the data

# STEP 3

Handle missing values

# STEP 4

Perform basic descriptive statistics

# STEP 5

Visualize the data

# CODE FOR “diabetes.csv”

import pandas as pd

import matplotlib.pyplot as plt

#load the diabetes dataset

diabetes_df = pd.read_csv("diabetes.csv")

#define a function for univariate analysis

def univariate_analysis(data, column):

#plot a histogram of the data

plt.hist(data[column], bins=10)

plt.xlabel(column)

plt.ylabel("Frequency")

plt.title(f"Histogram of {column}")

plt.show()

#plot a boxplot of the data

plt.boxplot(data[column])

plt.xlabel(column)

plt.ylabel("Value")

plt.title(f"Boxplot of {column}")

plt.show()

#print summary statistics of the data

print(f"Summary statistics of {column}:")

print(data[column].describe())

#perform univariate analysis on all specified columns

columns = ["Glucose", "BloodPressure", "SkinThickness", "Insulin", "BMI", "DiabetesPedigreeFunction", "Age", "Outcome"]

for col in columns:

  univariate_analysis(diabetes_df, col)

# OUTPUT

![image](https://user-images.githubusercontent.com/64436376/234244647-e50a4295-0a8f-437b-a71e-bd4e6d2a92f2.png)
![image](https://user-images.githubusercontent.com/64436376/234244687-496fe797-4620-47cd-b5ff-91784a2b110a.png)
![image](https://user-images.githubusercontent.com/64436376/234244712-090d3a7f-2118-4749-a87d-0fefaee9a082.png)
![image](https://user-images.githubusercontent.com/64436376/234244773-fa914dd2-41a0-4775-9795-ca5c6d6fb28c.png)
![image](https://user-images.githubusercontent.com/64436376/234245240-388eee3f-24af-4090-84c1-185b633daa24.png)
![image](https://user-images.githubusercontent.com/64436376/234245401-2b18a5f6-a53b-48af-84b9-e5be93d09c30.png)
![image](https://user-images.githubusercontent.com/64436376/234245560-f6b4ee10-0021-4d59-ba9d-91475feea135.png)
![image](https://user-images.githubusercontent.com/64436376/234245586-be8a8a19-0b2b-4d44-b5d7-b45b6efe9e94.png)
![image](https://user-images.githubusercontent.com/64436376/234245604-ac0233b8-686a-4c4d-a468-2a9b845b535a.png)
![image](https://user-images.githubusercontent.com/64436376/234245633-2b343a2d-a30d-4413-891f-ce226e9886f1.png)
![image](https://user-images.githubusercontent.com/64436376/234245651-89630939-9993-425e-b45e-ab9230da7c93.png)
![image](https://user-images.githubusercontent.com/64436376/234245679-bf72b23f-22d3-4bee-9636-901aec0e2eb2.png)
![image](https://user-images.githubusercontent.com/64436376/234245745-329cd2e8-2918-42dd-86c2-337c0e91056a.png)

# CODE FOR "SuperStore.csv"

import pandas as pd

import matplotlib.pyplot as plt

#load the SuperStore dataset

SuperStore_df = pd.read_csv("SuperStore.csv")

#define a function for univariate analysis

def univariate_analysis(data, column):

#plot a histogram of the data

plt.hist(data[column], bins=10)

plt.xlabel(column)

plt.ylabel("Frequency")

plt.title(f"Histogram of {column}")

plt.show()

#plot a boxplot of the data

plt.boxplot(data[column])

plt.xlabel(column)

plt.ylabel("Value")

plt.title(f"Boxplot of {column}")

plt.show()

#print summary statistics of the data

print(f"Summary statistics of {column}:")

print(data[column].describe())

#perform univariate analysis on all specified columns

columns = ["Row ID","Postal Code","Sales"]

for col in columns:

univariate_analysis(SuperStore_df, col)

# OUTPUT

![image](https://user-images.githubusercontent.com/64436376/234245944-22b89c11-e785-425c-92b9-cbc72ef3a5e9.png)
![image](https://user-images.githubusercontent.com/64436376/234245983-ba0936e6-fd17-4c03-bdf3-8a3e2652519b.png)
![image](https://user-images.githubusercontent.com/64436376/234246009-e8e52f2d-eccf-4da8-adf5-a77140e260df.png)
![image](https://user-images.githubusercontent.com/64436376/234246034-00ca7437-3a69-4e99-8c81-63d364b228ec.png)
![image](https://user-images.githubusercontent.com/64436376/234246064-8d733199-85f4-468c-bdc0-b1654e687877.png)
![image](https://user-images.githubusercontent.com/64436376/234246087-f3a3ee8e-08da-4a37-af77-7673738fdcaf.png)
![image](https://user-images.githubusercontent.com/64436376/234246112-1ec9e998-2534-4df2-b1ab-0892fd26e788.png)

# RESULT

Thus,to read the given data and perform Outlier Detection and Removal has been performed successfully.












