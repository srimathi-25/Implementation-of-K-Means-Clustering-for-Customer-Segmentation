# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import dataset and print head,info of the dataset

2.check for null values

3.Import kmeans and fit it to the dataset

4.Plot the graph using elbow method

5.Print the predicted array

6.Plot the customer segments

## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
Developed by: S.SRIMATHI
RegisterNumber: 212220040160

import pandas as pd

import matplotlib.pyplot as plt

data=pd.read_csv("/content/Mall_Customers (1).csv")

data.head()

data.info()

data.isnull().sum()

from sklearn.cluster import KMeans

wcss=[]

for i in range(1,11):

kmeans=KMeans(n_clusters=i,init="k-means++")

kmeans.fit(data.iloc[:,3:])

wcss.append(kmeans.inertia_)

plt.plot(range(1,11),wcss)

plt.xlabel("No_of_Clusters")

plt.ylabel("wcss")

plt.title("Elbow Method")

km=KMeans(n_clusters=5)

km.fit(data.iloc[:,3:])

y_pred=km.predict(data.iloc[:,3:])

y_pred

data["cluster"]=y_pred

df0=data[data["cluster"]==0]

df1=data[data["cluster"]==1]

df2=data[data["cluster"]==2]

df3=data[data["cluster"]==3]

df4=data[data["cluster"]==4]

plt.scatter(df0["Annual Income (k$)"],df0["Spending Score (1-100)"],c="red",label="cluster0")

plt.scatter(df1["Annual Income (k$)"],df1["Spending Score (1-100)"],c="black",label="cluster1")

plt.scatter(df2["Annual Income (k$)"],df2["Spending Score (1-100)"],c="blue",label="cluster2")

plt.scatter(df3["Annual Income (k$)"],df3["Spending Score (1-100)"],c="green",label="cluster3")

plt.scatter(df4["Annual Income (k$)"],df4["Spending Score (1-100)"],c="magenta",label="cluster4")

plt.legend()

plt.title("Customer Segment")
*/
```

## Output:
## DATA.HEAD():
![image](https://github.com/srimathi-25/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/114581999/ad279d34-66af-4d65-ba94-bd5d0e96947c)
## DATA.INF0():
![image](https://github.com/srimathi-25/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/114581999/fc25e209-debe-41e9-8c86-7fca16fa360f)
## DATA.ISNULL().SUM():
![image](https://github.com/srimathi-25/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/114581999/f0626442-2bc3-46a6-91a2-e7a6e5d4d275)
## PLOT USING ELBOW METHOD:
![image](https://github.com/srimathi-25/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/114581999/4d7a5d17-cbb1-454c-a6c1-20148cbc3ebf)
## K-MEANS CLUSTERING:
![image](https://github.com/srimathi-25/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/114581999/be9b0e77-f1d4-43ac-a63c-f8097321d35e)
## Y_PRED ARRAY:
![image](https://github.com/srimathi-25/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/114581999/a15f4350-9cd5-470c-afb3-49a9a98e797a)
## CUSTOMER SEGMENT:
![image](https://github.com/srimathi-25/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/114581999/6949fb52-0ffb-42eb-91f0-6c79a94efed0)


## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
