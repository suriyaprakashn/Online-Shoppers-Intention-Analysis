# Online Shoppers Intention Analysis

A comprehensive clustering analysis project to segment online shoppers based on their browsing behavior and purchasing intentions using session data from e-commerce websites.

## 📊 Project Overview

This project analyzes visitor browsing patterns on e-commerce sites to distinguish between users who are merely browsing and those likely to generate revenue. Using clustering techniques, we segment users to understand different behavioral patterns and optimize business strategies.

## 🎯 Objective

- Identify distinct clusters of online shoppers based on browsing behavior
- Compare clusters with the existing Revenue column for validation
- Understand characteristics of different user segments
- Provide insights for personalized marketing strategies

## 📁 Dataset Information

The dataset contains 12,330 sessions with 18 features (10 numerical, 8 categorical) representing user behavior on an e-commerce site.

### Attribute Description

| Feature | Description | Type |
|---------|-------------|------|
| Administrative | Number of administrative pages visited | Numerical |
| Administrative Duration | Time spent on administrative pages | Numerical |
| Informational | Number of informational pages visited | Numerical |
| Informational Duration | Time spent on informational pages | Numerical |
| Product Related | Number of product-related pages visited | Numerical |
| Product Related Duration | Time spent on product-related pages | Numerical |
| Bounce Rate | Percentage of single-page sessions | Numerical |
| Exit Rate | Percentage of exits from the page | Numerical |
| Page Value | Average value before transaction | Numerical |
| Special Day | Closeness to special days | Numerical |
| Month | Month of the visit | Categorical |
| Operating Systems | Visitor's OS | Categorical |
| Browser | Visitor's browser | Categorical |
| Region | Geographic region | Categorical |
| Traffic Type | Traffic source | Categorical |
| Visitor Type | New, Returning, or Other | Categorical |
| Weekend | Whether visit was on weekend | Boolean |
| Revenue | Whether session ended in purchase (Target) | Boolean |

## 🛠️ Technical Stack

- **Programming Language**: Python 3.8+
- **Data Manipulation**: Pandas, NumPy
- **Data Visualization**: Matplotlib, Seaborn, Plotly
- **Clustering Algorithms**: K-Means, DBSCAN, Hierarchical Clustering
- **Dimensionality Reduction**: PCA, t-SNE
- **Preprocessing**: Scikit-Learn preprocessing modules
- **Evaluation Metrics**: Silhouette Score, Davies-Bouldin Index


## 🔍 Exploratory Data Analysis

### Univariate Analysis
- Distribution of numerical features
- Frequency of categorical features
- Target variable (Revenue) distribution

### Bivariate Analysis
- Correlation between features and revenue
- Relationship between page types and conversion
- Time-based patterns (month, weekend)

### Multivariate Analysis
- Interaction between multiple variables
- Pattern recognition across feature combinations

## ⚙️ Data Preprocessing

### Missing Value Treatment
- Identification of missing values
- Appropriate imputation strategies

### Outlier Treatment
- Detection using IQR, Z-score methods
- Capping/transformation of outliers

### Feature Scaling
- Standardization of numerical features
- Normalization where appropriate

### Encoding Techniques
- One-hot encoding for categorical variables
- Label encoding for ordinal categories

## 🤖 Clustering Approach

### Algorithms to Implement
1. **K-Means Clustering** (Primary)
2. **DBSCAN** (Density-based)
3. **Hierarchical Clustering** (Agglomerative)

### Determining Optimal Clusters
- Elbow Method
- Silhouette Analysis
- Davies-Bouldin Index
- Gap Statistics

### Evaluation Metrics
- Silhouette Score
- Davies-Bouldin Index
- Calinski-Harabasz Index
- Cluster purity compared to Revenue labels

## 📊 Dimensionality Reduction

### Principal Component Analysis (PCA)
- Apply PCA to reduce dimensionality
- Evaluate explained variance ratio
- Perform clustering on PCA components
- Compare results with original feature clustering

### Visualization Techniques
- 2D/3D scatter plots of clusters
- t-SNE for high-dimensional visualization
- Parallel coordinates for cluster profiling
- Heatmaps of cluster centroids

## 🚀 Implementation Steps

1. **Data Loading and Understanding**
   - Load the dataset
   - Understand feature distributions and types

2. **Exploratory Data Analysis**
   - Univariate, bivariate, and multivariate analysis
   - Correlation analysis
   - Pattern identification

3. **Data Preprocessing**
   - Handle missing values and outliers
   - Encode categorical variables
   - Scale numerical features

4. **Clustering Analysis**
   - Determine optimal number of clusters
   - Apply multiple clustering algorithms
   - Evaluate cluster quality

5. **PCA Application**
   - Apply PCA for dimensionality reduction
   - Cluster on reduced dimensions
   - Compare with original clustering

6. **Cluster Interpretation**
   - Analyze cluster characteristics
   - Compare with Revenue column
   - Business insights generation

## 📈 Expected Outcomes

1. **Identified User Segments**: 3-5 distinct clusters of online shoppers
2. **Behavioral Patterns**: Characteristics of each user segment
3. **Conversion Insights**: Understanding what drives purchases
4. **Actionable Recommendations**: Strategies for each user segment
5. **Model Evaluation**: Quality metrics for clustering performance

## 💼 Business Applications

- **Personalized Marketing**: Tailored campaigns for different segments
- **User Experience Optimization**: Customized browsing experience
- **Conversion Rate Optimization**: Targeted strategies for likely buyers
- **Resource Allocation**: Focus on high-value user segments
- **Customer Retention**: Strategies for different visitor types



## 🤝 Contributing

We welcome contributions! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- UCI Machine Learning Repository for the dataset
- Original researchers: Sakar, C.O., Polat, S.O., Katircioglu, M. et al.
- Open-source community for machine learning libraries

---

**Note**: This project provides insights into user behavior patterns but should be complemented with domain knowledge for business implementation. The clustering results are data-driven suggestions that can inform but not replace business strategy decisions.
