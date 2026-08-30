# Customer Segmentation using K-Means Clustering

A hands-on machine learning practice project focused on **customer segmentation using K-Means clustering**.

The project uses the **Mall Customer Segmentation Data** dataset and explores how customers can be grouped based on their **annual income** and **spending score**.

## Project Overview

Customer segmentation is an unsupervised learning task that groups customers with similar characteristics.

In this project, K-Means clustering is applied to identify groups of customers based on:

* Annual Income
* Spending Score

The project also uses the **Elbow Method** to help determine an appropriate number of clusters and compares clustering results for different values of K.

## Dataset

The project uses the **Mall Customer Segmentation Data** dataset from Kaggle.

Dataset source:

https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python

The dataset is downloaded directly through the Kaggle API in the notebook.

The analysis uses the following features:

| Feature                | Description                                      |
| ---------------------- | ------------------------------------------------ |
| Annual Income (k$)     | Customer's annual income in thousands of dollars |
| Spending Score (1-100) | Customer spending score                          |

## Methodology

The project follows this workflow:

```text
Mall Customer Dataset
        ↓
Load Dataset
        ↓
Select Relevant Features
        ↓
Visualize Customers
        ↓
Elbow Method
        ↓
Select K = 5
        ↓
Apply K-Means Clustering
        ↓
Analyze Cluster Distribution
        ↓
Compare K = 4, 5, and 6
```

### 1. Dataset Loading

The Mall Customers dataset is downloaded from Kaggle and loaded into a Pandas DataFrame.

The notebook also displays the dataset and the total number of customers.

### 2. Feature Selection

Two features are selected for clustering:

```text
Annual Income (k$)
Spending Score (1-100)
```

These features are used to represent customers in a two-dimensional feature space.

### 3. Visualization Before Clustering

A scatter plot is created to visualize the relationship between annual income and spending score before applying clustering.

### 4. Elbow Method

The Elbow Method is used to evaluate different values of K.

The notebook calculates K-Means inertia for:

```text
K = 1 to 10
```

The resulting inertia values are visualized using an elbow plot to help identify a suitable number of clusters.

### 5. K-Means Clustering

The main clustering experiment uses:

* Algorithm: K-Means
* Number of clusters: **5**
* Random state: **42**

Each customer is assigned a cluster label, and the cluster assignments are added to the original dataset.

### 6. Cluster Visualization

The resulting five clusters are visualized using a scatter plot.

The plot displays:

* Individual customers
* Cluster groups
* Cluster centers

This provides a visual representation of how customers are separated according to annual income and spending score.

### 7. Cluster Summary

The notebook calculates the mean annual income and spending score for each cluster.

It also reports the number of customers assigned to each cluster.

### 8. K Comparison

To further explore the clustering structure, K-Means is also evaluated visually using:

* K = 4
* K = 5
* K = 6

This allows the clustering behavior to be compared across different numbers of clusters.

## Technologies & Libraries

* Python
* Pandas
* Matplotlib
* Scikit-learn
* K-Means Clustering
* Kaggle API
* Google Colab

## Repository Structure

```text
customer-segmentation-kmeans/
│
├── Customer_Segmentation_using_K_Means_Clustering.ipynb
├── README.md
└── .gitignore
```

The dataset itself is not included in the repository because it is downloaded from Kaggle through the notebook.

## How to Run

### Google Colab

Open the notebook in Google Colab and execute the cells sequentially.

The notebook requires Kaggle API credentials to download the dataset.

**Important:** Do not upload or commit your `kaggle.json` file to GitHub.

### Local Environment

Install the required libraries:

```bash
pip install pandas matplotlib scikit-learn kaggle
```

Then configure your Kaggle API credentials and run the notebook using Jupyter Notebook or JupyterLab.

## Key Learning Outcomes

This project was developed as hands-on practice to strengthen understanding of:

* Unsupervised learning
* K-Means clustering
* Customer segmentation
* Feature selection for clustering
* The Elbow Method
* Cluster visualization
* Cluster centers
* Inertia
* Comparing different values of K
* Interpreting cluster distributions

## Future Improvements

Possible extensions include:

* Standardizing features before clustering
* Evaluating clusters using the Silhouette Score
* Testing additional clustering algorithms
* Performing more systematic K selection
* Including additional customer attributes
* Creating detailed customer segment profiles
* Developing a dashboard for interactive customer segmentation

 

GitHub: https://github.com/YOUR-USERNAME
