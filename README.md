1.Data Loading and Preprocessing:
  *Reads the customer data from a CSV file named "Mall_Customers.csv" using pandas.
  *Selects the relevant features for clustering: 'Age', 'Annual Income (k$)', and 'Spending Score (1-100)'.
  *Scales the features using StandardScaler to standardize them.

2.Determination of Optimal Number of Clusters:
  *Iterates over a range of cluster numbers (from 2 to 10).
  *Performs K-means clustering for each number of clusters.
  *Calculates the silhouette score for each clustering.
  *Plots the silhouette scores against the number of clusters to determine the optimal number of clusters.

3.Clustering:
  *Uses the optimal number of clusters determined from the silhouette scores to perform K-means clustering again.
  *Assigns cluster labels to each data point.
  *Adds a new column 'Cluster' to the original data to indicate the cluster each customer belongs to.

4.Visualization:
  *Visualizes the clustering result by plotting the 'Annual Income' against 'Spending Score' for each cluster.
  *Also plots the centroids of each cluster.

5.Output:
  *Prints the cluster labels assigned to each customer along with their CustomerID.
  
To run this code:

Create a Python file named "main.py" and paste the provided code into it.
Make sure the "Mall_Customers.csv" dataset file is in the same directory as "main.py".
Execute the "main.py" file using a Python interpreter.
Follow the instructions provided by the program to interpret the clustering results.
Ensure that the dataset directory is correctly specified in the code. Additionally, customize the dataset by adjusting the column names and data accordingly in the CSV file.
