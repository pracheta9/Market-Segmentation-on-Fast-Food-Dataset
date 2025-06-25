# Market-Segmentation-on-Fast-Food-Dataset

## 🧠 McDonald's Market Segmentation Analysis
This project applies advanced market segmentation techniques on a fast-food consumer dataset related to McDonald’s. The goal is to identify meaningful consumer clusters using unsupervised learning methods and to profile them based on their perceptions and preferences. The analysis was originally demonstrated in R, and this project fully replicates and extends the logic using Python.

### 📊 Project Objective
To segment McDonald’s customers based on their opinions (e.g., "tasty", "greasy", "convenient") using:

Binary clustering (k-means, LCA)

Principal Component Analysis (PCA)

Mosaic and bar plots for profiling

Segment stability and evaluation techniques

### 🧰 Libraries Used

pandas, numpy: data manipulation
matplotlib, seaborn: visualizations
sklearn: PCA, k-means, label encoding, cluster evaluation
statsmodels.graphics.mosaicplot: mosaic plots
scipy.cluster.hierarchy: hierarchical clustering
bioinfokit: cluster visualization (optional)
plotly.express: enhanced visualizations (optional)

### 🧾 Dataset
The dataset used (mcdonalds.csv) contains:

11 binary columns representing consumer perceptions (e.g., yummy, cheap, spicy)

Descriptor variables like Like, Gender, Age, VisitFrequency

### 📌 Key Steps
1. Data Preparation
Encoded "Yes"/"No" responses into binary (1/0)

Calculated response proportions to visualize perceptions

2. Dimensionality Reduction
Applied PCA to visualize and interpret perceptual mapping

Plotted perceptual maps using projected components

3. Segmentation Techniques
K-means clustering: performed with 2–8 clusters and elbow method

Stability analysis: bootstrapped adjusted Rand Index to test reproducibility

Latent Class Analysis (LCA): implemented using mixture models for binary data

4. Segment Profiling
Segment profile bar charts with attributes reordered using hierarchical clustering

Mosaic plots for segment vs "Like" response

Evaluation plots to relate cluster-level preferences to visit frequency

5. Visualizations
PCA perceptual maps

Segment-wise bar charts and heatmaps

Mosaic plots (segment × gender, segment × like)

### 📈 Outputs
Cluster Profile Charts: Visual comparison of how each cluster feels about McDonald’s (e.g., Cluster 1 finds it greasy and cheap).

Mosaic Plot: Visual relationship between clusters and liking/disliking McDonald's.

Segment Evaluation: Understanding how often each cluster visits and how much they like McDonald’s.

### 📈 Insights
Convenience is universally perceived positively (91%).

Spiciness and healthiness are perceived least positively.

Segments differ in perceptions of taste, cost, and healthiness.

Clear differences across clusters in how much they like McDonald’s.
