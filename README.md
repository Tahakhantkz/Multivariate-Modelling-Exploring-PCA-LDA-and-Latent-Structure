# Multivariate Modelling: Exploring PCA, LDA and Latent Structure

## About the Project

This project explores some interesting concepts in multivariate modelling, particularly how dimensionality reduction techniques can help us understand complex datasets.

Developed as part of the **STAT9014 – Multivariate Modelling** module, the project uses the Breast Cancer Wisconsin dataset to explore Principal Component Analysis (PCA), Linear Discriminant Analysis (LDA), and the relationship between variance and useful information.

The project also explores a different perspective on PCA by looking at observations along the first principal component, rather than using PCA solely as a dimensionality reduction technique.

## Dataset

The analysis uses the **Breast Cancer Wisconsin dataset**, which contains measurements derived from digitized images of breast mass cell nuclei.

The dataset includes 30 features describing characteristics such as:

- Radius
- Texture
- Perimeter
- Area
- Smoothness
- Compactness
- Concavity
- Symmetry

These measurements help distinguish between benign and malignant cases.

## What I Explored

### 1. When PCA Doesn't Work as Expected

I initially explored the Online News Popularity dataset, expecting PCA to reveal meaningful underlying structure.

However, the scree plot did not show a clear elbow, and the variance was spread across many components. This was an interesting starting point because it highlighted that PCA does not always provide substantial dimensionality reduction.

This experience helped me understand that PCA reveals existing structure in the data rather than creating structure where none is apparent.

### 2. Variance Is Not the Same as Information

Using the Breast Cancer dataset, I explored PCA and LDA to understand how they approach dimensionality reduction differently.

- **PCA:** Reduced the original 30 features to 4 principal components while retaining approximately 81% of the variance.
- **LDA:** Reduced the data to a single dimension while achieving strong class separation.

This comparison highlighted an important idea: the directions that explain the most variance are not necessarily the directions that best separate classes.

### 3. PC1 as a Latent Trajectory

Instead of only looking at how much variance PC1 explains, I explored whether it could be used to organize observations along a continuous axis.

By sorting observations according to their PC1 scores, I explored a possible progression within the dataset and how dimensionality reduction can provide a different way of interpreting data.

## Key Takeaways

- A model that fails to reveal structure can still provide valuable statistical insight.
- Explained variance does not necessarily represent the most useful information for classification.
- PCA and LDA serve different purposes and can provide complementary perspectives.
- Principal components can be used to explore patterns and organize observations, beyond simply reducing the number of features.

## Tools and Techniques

- Python
- PCA (Principal Component Analysis)
- LDA (Linear Discriminant Analysis)
- Variance analysis
- Scree plots
- Correlation analysis
- Data visualization

## Dataset Source

Breast Cancer Wisconsin dataset – UCI Machine Learning Repository.

## Academic Context

**Module:** STAT9014 – Multivariate Modelling  
**Programme:** MS Data Science and Analytics

