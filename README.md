# Clustering-with-K-Means


##  Objective

The goal of this project is to apply **unsupervised learning** using **K-Means clustering** to segment customers based on their behavior.
We use the **Mall Customer Segmentation Dataset** to identify distinct customer groups that can help businesses with targeted marketing strategies.

---

##  Tools & Libraries

* **Python**
* **Pandas** → Data handling
* **Matplotlib / Seaborn** → Data visualization
* **Scikit-learn** → K-Means, PCA, Silhouette Score

---

## Dataset

**Mall_Customers.csv**

* `CustomerID`
* `Gender`
* `Age`
* `Annual Income (k$)`
* `Spending Score (1-100)`

For clustering, we mainly use **Annual Income** and **Spending Score**.

---

##  Steps Performed

1. **Load & Explore Dataset**

   * Imported dataset using Pandas.
   * Visualized feature distributions.

2. **Feature Selection**

   * Used `Annual Income (k$)` and `Spending Score (1-100)` as input features.

3. **Elbow Method**

   * Computed Within-Cluster Sum of Squares (WCSS) for k=1 to 10.
   * Choose optimal k=5 from the "elbow point".

4. **K-Means Clustering**

   * Fit K-Means with 5 clusters.
   * Assigned each customer a cluster label.

5. **Visualization**

   * Plotted customer clusters with different colors.
   * Marked centroids with red "X".
   * (Optional) Used PCA for dimensionality reduction when >2 features.

6. **Evaluation**

   * Computed **Silhouette Score = 0.55**
   * Interpretation: Clusters are well-formed and meaningful (good separation).

---

##  Customer Segments (5 Clusters)

1. **Low Income – Low Spending** → Thrifty customers
2. **Low Income – High Spending** → Carefree / Loyal shoppers
3. **High Income – Low Spending** → Potential customers (conservative)
4. **High Income – High Spending** → Premium / VIP customers
5. **Average Income – Average Spending** → Middle-class customers

---

##  Key Insights

* K-Means successfully segmented customers into **5 distinct groups**.
* The Silhouette Score suggests a **good clustering structure**.
* These groups can be used for **targeted marketing strategies** (e.g., loyalty programs for Cluster 2, VIP services for Cluster 4, promotional offers for Cluster 3).

---



##  Results

The project demonstrates how unsupervised learning can uncover **hidden patterns in customer behavior** and help businesses make **data-driven decisions**.
