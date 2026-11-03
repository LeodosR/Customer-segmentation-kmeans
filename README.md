# Customer-segmentation-kmeans
Tools used: Python, pandas, NumPy, scikit-learn, Matplotlib/Seaborn.

Customer Segmentation: E-commerce Orders

**Goal:** Group customers by purchasing behaviour so that marketing can be targeted at each group rather than at everyone.

**Data:** About 950,000 order lines from an international retailer, covering customers in 47 countries across five continents between 2012 and 2016. Each row holds details about the order (dates, quantity, revenue, cost, discount, profit) and the customer (location, loyalty group, birthdate). Source: SAS, 2024. CUSTOMERS_CLEAN [Data set]. SAS. Last revised on 15 December 2021. [Accessed 20 February 2024].

**Approach:**

Cleaned the data and engineered customer-level features: recency, frequency, customer lifetime value, average unit cost and age.

Chose the optimal number of clusters (4) using the Elbow Method, Silhouette Scores and hierarchical clustering.

Segmented customers with K-Means, and used PCA and t-SNE to visualise and interpret the groups.

**Outcome:** Identified 4 key customer segments, including high spenders, older and younger customers and a cluster of new clientel. As t-SNE visualised our resulting cluster better than PCA (which we can attribute to non-linearity), with a perplexity level of 50, it demonstrated clearly separated our 'champs' and 'fresh catch' clusters, while out younger and older categories show marginal ovelapping.

Identified clusters:

- Cluster 1:  Lapsed-Youth

This is clearly the youngest cluster group as shown by the age range, and elsewhere, this cluster sits moderately amongst the other features.

- Cluster 2: The champs

This cluster is notable for the higher frequency and CLV rating when compared to the other groups. In these features they also display high levels of outliers, reaffirming the value of this group. It also has the highest IQR for average unit cost, suggesting a higher likliehood of mid-to high range purchses.

- Cluster 3: Fresh catch

This cluster demonstrates the most recent customer base by a large profile. This would seem logical through the lower frequency and CLV rankings of this cluster. It also represents a diverse range of customers due to the wide age range.

- Cluster 4: Veterans

This cluster is notable for its older age range and alike to cluster 1, sits relatively similarly in terms of the other features.

<img width="887" height="590" alt="download" src="https://github.com/user-attachments/assets/386cfe07-92df-4997-936e-29bcc2687624" />

Source:
SAS, 2024. CUSTOMERS_CLEAN [Data set]. SAS. Last revised on 15 December 2021. [Accessed 20 October 2026].
