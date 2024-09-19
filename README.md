
---

# Customer Segmentation Using RFM Analysis and K-Means Clustering

This project demonstrates customer segmentation using **RFM analysis** and **K-Means clustering**. The goal is to identify key customer groups based on their purchasing behavior and to provide actionable insights for targeted marketing strategies.

## Project Overview

Customer segmentation is crucial for understanding customer behavior and creating personalized marketing strategies. In this project, we used RFM (Recency, Frequency, and Monetary) analysis to group customers and applied K-Means clustering to segment them into distinct clusters.

### Tools & Technologies
- **Python**: Main programming language used.
- **Pandas**: For data manipulation and cleaning.
- **Scikit-Learn**: For K-Means clustering.
- **Matplotlib & Seaborn**: For data visualization.
  
### Dataset
The dataset used for this analysis is the **Online Retail Dataset**, available from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Online+Retail). It contains transactions of a UK-based online retail store over the course of a year.

## Steps in the Project

1. **Data Cleaning**:
   - Removed rows with missing `CustomerID` and irrelevant `InvoiceDate`.
   - Handled missing values in the dataset and created necessary features like `TotalSpent`.

2. **RFM Feature Engineering**:
   - **Recency**: How recently a customer made a purchase.
   - **Frequency**: How often a customer makes a purchase.
   - **Monetary**: How much money a customer has spent.

3. **Scaling the Data**:
   - Used `StandardScaler` to standardize the RFM features before applying clustering.

4. **Clustering**:
   - Determined the optimal number of clusters using the **Elbow Method** and **Silhouette Score**.
   - Applied **K-Means clustering** to segment customers into distinct groups.

5. **Visualization**:
   - Visualized the clusters using scatter plots to interpret relationships between **Recency**, **Frequency**, and **Monetary** values.

6. **Insights**:
   - Analyzed each cluster to provide insights into customer behavior and proposed marketing strategies.

## Key Results and Insights

### Cluster 0: **Engaged, Frequent Buyers**
- **Recency**: 43.75 (recently engaged).
- **Frequency**: 22.6 (frequent purchasers).
- **Monetary**: 12,405.58 (moderate spenders).
- **Insight**: Steady, loyal customers. Focus on retaining them with special offers.

### Cluster 1: **High-Value, VIP Customers**
- **Recency**: 24.00 (highly engaged).
- **Frequency**: 82.69 (extremely frequent purchasers).
- **Monetary**: 127,187.96 (very high spenders).
- **Insight**: These are your top customers. Reward them with exclusive offers or loyalty programs.

### Cluster 2: **At-Risk or Inactive Customers**
- **Recency**: 357.37 (haven’t purchased in almost a year).
- **Frequency**: 2.57 (low-frequency buyers).
- **Monetary**: 865.07 (low spenders).
- **Insight**: These customers are at risk of churning. Consider running win-back campaigns to re-engage them.

### Cluster 3: **Low-Value, Infrequent Buyers**
- **Recency**: 100.46 (not very recent).
- **Frequency**: 4.33 (infrequent buyers).
- **Monetary**: 1,578.44 (low spenders).
- **Insight**: These are low-value customers. Encourage higher engagement through personalized promotions.

## How to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/abdoolamunir/Customer-Segmentation-Using-RFM-Analysis-and-K-Means-Clustering.git
   ```
   
2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook Clustering.ipynb
   ```

4. Explore the clustering results and visualizations.

## Future Enhancements
- **Automate customer updates**: Build a pipeline that can automatically update customer clusters based on new data.
- **Deploy as a web app**: Deploy the clustering results and insights via a dashboard for business users to interact with.
- **Explore other clustering techniques**: Investigate other clustering methods such as Hierarchical Clustering or DBSCAN for comparison.

## Conclusion

This project successfully segmented customers into meaningful groups using RFM analysis and K-Means clustering. The insights derived can be used to create targeted marketing strategies, improve customer engagement, and increase business revenue.

---

Feel free to modify this based on any additional details or specific features of your project. Let me know if you need any further changes or assistance!
