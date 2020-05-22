# USDAFoodCompositionAnalysis

 
Problem Statement:

Analyze USDA food composition data for Vitamins, Minerals and Macronutrients.

1. Cluster identification- Is it possible to group the foods into distinct clusters according to how similar they are across all macronutrients, vitamins and minerals quantities recorded in the data?


2. Clusters vs. labels. Once a set of clusters has been found, how do the clusters compare to the food groups recorded in the data (e.g., Poultry, Dairy and Egg, Fruits) (see the field “FdGrp_Desc”)?
Do food belonging to the same food group fall in the same clusters?
Are there foods that belong to the same food group but fall into different clusters (that is, same food group but different food composition)?
Are there foods that belong to different groups but fall into the same cluster (that is, different food groups but similar food composition)?

3. Outliers. Are there any foods that tend to be different from all the others (that is, they are outliers)? What is unique about them? What makes them unique?


4. Interpretation. For the clusters and outliers identified above, what aspects of their food composition make them different from the others and similar to the food that belong to the same cluster (that is, what makes a cluster (or outlier) unique in terms of their data values and distribution and how does it compare to the other clusters)?



Analysis:


# Clustering:

We ran TSNE on the dataset with the relevant columns, and identified clusters via K-means clustering. Elbow method was used to identify optimal cluster number: k=12

After TSNE :

### Clustering by Vitamins :

![Clusters](/images/visualization-106.png)

### Clustering by Minerals :

![Clusters](/images/visualization-113.png)

### Clustering by Macronutrients :

![Clusters](/images/visualization-120.png)



# Clusters Explained By Its Nutrients:

We plotted the median of all nutrients in a cluster to analyze the cluster wise spread of nutrients. The data was normalized in preprocessing stage.


### Vitamins Clusters explained :

![Clusters](/images/visualization-108.png)

### Minerals Clusters explained :

![Clusters](/images/visualization-115.png)

### Macronutrients Clusters explained : :

![Clusters](/images/visualization-122.png)



# How do Clusters compare to different foodgroups:

![Vitamins](/images/visualization-107.png)  ![Minerals](/images/visualization-114.png). ![Macronutrients](/images/visualization-121.png).

