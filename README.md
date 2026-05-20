# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. The program loads the mall customer dataset and extracts the annual income and spending score features.
2. It initializes a K-Means clustering model configured to divide the data into 5 distinct groups.
3. The model fits the data and predicts cluster assignments for every individual customer.
4. It generates a scatter plot where customers are color-coded based on their assigned cluster.
5. Finally, it overlays large 'X' markers to pinpoint the exact centroids of each of the 5 clusters.
 
## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.

import pandas as pd
import matplotlib.pyplot as plt
from sklearn.cluster import KMeans

data = pd.read_csv("Mall_Customer.csv")

X = data.iloc[:, [3, 4]].values

kmeans = KMeans(n_clusters=5, random_state=0)

y_kmeans = kmeans.fit_predict(X)

plt.scatter(X[:, 0], X[:, 1], c=y_kmeans, s=50)

plt.scatter(kmeans.cluster_centers_[:, 0],
            kmeans.cluster_centers_[:, 1],
            s=200,
            marker='X')

plt.xlabel("Annual Income")
plt.ylabel("Spending Score")
plt.title("Customer Segmentation using K-Means")

plt.show()

Developed by: K SAKTHIVEL 
RegisterNumber:  212225240133
*/
```

## Output:

<img width="806" height="606" alt="594472027-25c17ca8-913a-4dea-bf25-3f29e73e42aa" src="https://github.com/user-attachments/assets/9ef747cc-b4db-4016-8e4c-7c1d77c70723" />

## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
