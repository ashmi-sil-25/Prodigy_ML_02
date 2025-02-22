# **CUSTOMER SEGMENTATION USING K-MEANS CLUSTERING** #

### 1. Importing Libraries ###
- Loads necessary libraries for data handling (`pandas`, `numpy`), visualization (`matplotlib`, `seaborn`), and machine learning (`sklearn`).

### 2. Setting Environment Variable ###
- Limits the number of processing threads to 1 to avoid parallel execution issues with K-Means.

### 3. Loading the Dataset ###
- Reads the customer data from a CSV file into a Pandas DataFrame.

### 4. Displaying the Data ###
- Checks the structure of the dataset by viewing the first few rows.

### 5. Selecting Features for Clustering ###
- Extracts "Annual Income" and "Spending Score" as the key features for customer segmentation.

### 6. Standardizing the Data ###
- Scales the selected features to have zero mean and unit variance to ensure better performance of the clustering algorithm.

### 7. Finding the Optimal Number of Clusters (Elbow Method) ###
- Runs K-Means for different cluster values (k = 1 to 10).
- Computes **Within-Cluster Sum of Squares (WCSS)** for each value of k.
- Stores WCSS values to determine the best number of clusters.
  
### 8. Plotting the Elbow Curve ###
- Creates a graph of WCSS vs. number of clusters.
- The **"elbow" point** (where the WCSS drop slows down) suggests the optimal number of clusters.
  
### 9. Applying K-Means Clustering ###
- Uses the optimal number of clusters (k=5).
- Assigns each customer to a cluster based on their spending behavior and income.
  
### 10. Adding Cluster Labels to the Dataset ###
- Saves the assigned cluster number for each customer in the original dataset. 

### 11. Visualizing the Clusters ###
- Plots the customer groups using a scatter plot.
- Different colors represent different clusters.
- Red "X" markers indicate the cluster centroids (center points).

### 12. Final Output ### 
- The customers are now grouped into five distinct clusters based on their annual income and spending score, helping the retail store analyze customer behavior for better marketing strategies.

## Key Objective: ##
To segment customers of a retail store into distinct groups based on their **Annual Income** and **Spending Score** using the **K-Means clustering algorithm**. This helps in identifying different customer behaviors, enabling targeted marketing strategies and personalized customer engagement.
