# Scalable Recommendation System with PySpark on GCP

This project involves building a scalable recommendation system using `Google Cloud Platform (GCP)` and `PySpark` enhanced with `K-Means clustering` to improve recommendation quality. The approach leverages distributed computing for efficient handling of large datasets while employing clustering techniques to group users or items for personalized suggestions.
<br>
<br>
## Overview
1. **Cloud Storage Setup**
  - Configured Google Cloud Storage for data storage and retrieval.
3. **PySpark Implementation**
  - Employed Spark API calls to utilize Python's capabilities with PySpark.
  - Utilized both in-memory and disk computations for faster data processing.
3. **K-Means Clustering**
  - Applied K-Means to group users or items into clusters based on their features.
  - Helped refine the recommendation system by suggesting items from the same cluster, enhancing personalization.
  - Used an elbow plot to determine the optimal number of clusters by minimizing distortions.
4. **Collaborative Filtering**
  - Incorporated user-item interaction matrices to predict preferences using advanced techniques like matrix factorization.

### Visual Insights
- Elbow Method Plot: Displayed distortions for different cluster sizes (k = 4; wrt to this project) to identify the optimal number of clusters for K-Means. <br>
![Screenshot 2025-01-05 at 5 35 53 PM](https://github.com/user-attachments/assets/e58c4313-970d-4e3b-997e-b1729d40b84e)

- Cluster Visualization: Plotted data points grouped into clusters using different colors, with centroids marked for better interpretability. <br>
![Screenshot 2025-01-05 at 5 39 12 PM](https://github.com/user-attachments/assets/20a7ff3c-9d18-4d50-bdf9-d18c708d03db)

- Recommendation Quality: Highlighted how clustering reduces noise and improves the relevance of recommendations.<br>
![Screenshot 2025-01-05 at 5 40 02 PM](https://github.com/user-attachments/assets/2d7b6e13-0d03-4b2e-91e5-b395c25cb61b)

### Implementation Highlights
1. **Clustering with K-Means**

  - Segmented data into meaningful clusters based on features like user preferences, genres, or ratings.
  - Visualized the clusters for interpretability and verified optimal grouping using centroid analysis.
2. **Recommendation Algorithm**

  - Defined a utility function to retrieve recommendations based on a user’s cluster.
  - Allowed queries by book title or ID, fetching highly relevant recommendations by analyzing clustered neighbors.
