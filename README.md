# Customer Segmentation Using RFM Analysis Combined With K-Means Clustering

## Project Introduction
 <p>
   The goal of this project is to segment customers based on their purchasing behavior using RFM (Recency, Frequency, Monetary) analysis combined with K-Means clustering. By understanding different customer segments, businesses can tailor their marketing strategies to target each segment effectively, ultimately improving customer retention and increasing revenue.
 </p>

## Objectives
<ul>
  <li>
    Perform RFM analysis to quantify customer behavior.
  </li>
  <li>
    Use K-Means clustering to segment customers based on their RFM scores.
  </li>
  <li>
    Interpret the resulting customer segments and provide actionable insights for business strategy.
  </li>
</ul>

## Dataset
<p>
  The dataset I used is from an open dataset on BigQuery. Here is the link where you can access the dataset.
</p>

## Methodology
1. Data Preprocessing
   <ul>
     <li>
       Data Cleaning: Checking duplicate, handling missing data, and drop the data that not related with the analysis
     </li>
   </ul>
2. RFM Analysis
   <ul>
     <li>
       Recency (R): Calculate the number of days since the customer's last purchase.
     </li>
     <li>
       Frequency (F): Count the total number of purchases made by the customer.
     </li>
     <li>
       Monetary (M): Sum the total monetary value of all purchases made by the customer.
     </li>
   </ul>
3. Normalization
   <ul>
     <li>
       Normalize the RFM values to ensure each metric has equal influence during clustering. This can be done using Standardization.
     </li>
   </ul>
4. K-Means Clustering
   <ul>
     <li>
        Determine Optimal Number of Clusters: Use Silhouette analysis and Davies-Bouldin index to identify the optimal number of clusters (k).
     </li>
     <li>
       Clustering: Apply K-Means clustering to the normalized RFM scores to segment customers into distinct groups.
     </li>
     <li>
       Cluster Profiling: Analyze each cluster to understand the characteristics of the customers within it.
     </li>
   </ul>

## Recommendation

**For Passive Customer**
  1.   The company can offer incentives such as coupons or gifts to encourage repeat purchases.
  2.   The company can run email marketing campaigns to re-engage their attention.
  3.   Offer relevant products or services based on previous purchase history to increase interest and purchase frequency.

**For Loyal Customer**
  1.   The company can implement a loyalty program that offers points or discounts to loyal customers.
  2.   The company can take the opportunity to upsell more expensive products or cross-sell additional products. Offer special deals or product bundles.

**For New Potential Customer**
  1.   The company can provide education about the products and their benefits through email or valuable content.
  2.   The company can offer promotions that increase transaction value, such as product bundles or discounts for bulk purchases.
