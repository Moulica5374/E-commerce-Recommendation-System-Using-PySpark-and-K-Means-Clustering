# E-commerce-Recommendation-System-Using-PySpark and K-Means-Clustering | PCA

This project demonstrates how to build a scalable recommendation system using PySpark. It focuses on clustering-based recommendations by processing product data(PySpark), extracting embeddings(Open AI text embeddings), applying dimensionality reduction(PCA) and generating product clusters to offer intelligent suggestions based on user behavior.

- Fetch the api keys from the open ai in order to use it for text embeddings and secure it .

- Dimensionality reduction using Principal Component Analysis (PCA) to retain meaningful features while reducing vector size.

- Text preprocessing by combining product titles and descriptions to generate embedding vectors.

- Product clustering using K-Means to identify similar items.

- Cluster visualization after PCA transformation for interpretability.

- User behavior analysis by filtering recently viewed items.

- Recommendation logic based on similarity within product clusters.

- Optimization of PySpark joins using partitioning and data shuffling strategies.

## Tools and Technologies

- PySpark for large-scale data processing

- VectorAssembler for combining features into vectors

- PCA for dimensionality reduction

- K-Means for clustering similar items

- Python .env management for secure configuration

 - matplotlib for data visualization

## Key Takeaways
Environment Setup
- Used .env files for secure key storage and reproducible configuration.

- Enabled scalable processing through SparkSession and distributed dataframes.

Data Preparation
- Utilized concat_ws to concatenate product titles and descriptions.

- Extracted embedding vectors that encode semantic and contextual information.

Clustering and Dimensionality Reduction
- Used VectorAssembler to prepare features for machine learning.

- Applied K-Means clustering to group similar products.

- Performed PCA to reduce high-dimensional embeddings for visualization and analysis.

## Behavior-Based Filtering

- Filtered user activity logs to focus on recently viewed products.

- Processed data using parallel RDDs for scalability and performance.

Recommendation Logic
- Clustered items were used to recommend similar products.

- Applied ranking and similarity metrics within clusters to enhance accuracy.

Performance Optimization
- Addressed overheads in joins using smart repartitioning and shuffling.

- Minimized data movement across nodes by partitioning on join keys.

## Skills Demonstrated

- PySpark-based distributed machine learning

- Real-time, behavior-aware recommendations

- Unsupervised learning with K-Means

- Dimensionality reduction using PCA

- Scalable pipeline design and optimization


## Future Work

- Integrate real-time event streams using Apache Kafka or AWS Kinesis to update recommendations on-the-fly.
- Replace K-Means with more advanced algorithms such as DBSCAN, hierarchical clustering, or ALS (Alternating Least Squares) for collaborative filtering.
- Deploy the recommendation engine as a microservice with REST APIs using Flask or FastAPI.
- Store and serve personalized recommendations using scalable databases like Amazon DynamoDB or Redis.
- Implement session-based or sequence-aware recommendations using Recurrent Neural Networks (RNNs) or Transformer architectures.
- Build an interactive dashboard using Streamlit or Dash to visualize clusters, embeddings, and user behavior in real time.
- Apply A/B testing to evaluate different recommendation strategies and optimize for user engagement.
