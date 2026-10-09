# Unsupervised-Dominant-Colour-Detection
An unsupervised machine learning project that uses K-means clustering to identify dominant colours in images, visualize pixel distributions in RGB space, and compare clustering results using the Xie–Beni Index.

# Overview
This project explores unsupervised learning for image colour analysis using K-means clustering. By representing image pixels as points in three-dimensional RGB colour space, the algorithm groups similar colours into clusters and identifies their corresponding cluster centers.

The project investigates how different numbers of clusters and initial centroid positions affect the clustering results.

# Objectives
- Implement K-means clustering to group image pixels based on RGB colour values.
- Visualize pixel distributions and cluster-centroid movements in 3D RGB space.
- Generate simplified images by assigning pixels to their corresponding cluster colours.
- Compare clustering solutions using the Xie–Beni Index.

# Technologies Used
- Python
- Jupyter Notebook
- NumPy
- Matplotlib
- K-means clustering
- Xie–Beni cluster validity index

# Methodology
1. RGB Colour-Space Representation

   Image pixels are represented as points in a three-dimensional space, with red, green, and blue intensity values forming the three    axes. This representation allows the distribution of colours within an image to be visualized and analyzed.

2. K-Means Clustering
   
   K-means clustering groups pixels according to their distances from cluster centers. The algorithm iteratively assigns pixels to      their nearest cluster and updates the centers until convergence.
  
   Experiments were conducted using two and five clusters to investigate how the number of clusters affects the resulting colour        segmentation.

3. Visualization and Evaluation

   The project visualizes cluster-centroid movements during iterations and generates images in which pixels are represented by their    assigned cluster colours.

   Two five-cluster experiments were also conducted using different random seeds. Their results were compared using the Xie–Beni        Index, which provides a measure for evaluating clustering quality.

# Results
- The two-cluster experiment grouped image pixels into two colour categories.
- Two five-cluster experiments converged after 19 and 16 iterations, respectively.
- The resulting five-cluster solutions were visually similar, although the cluster labels differed.
- The Xie–Beni Index was approximately 0.21409 for Run 1 and 0.21421 for Run 2. Run 1 achieved the slightly lower index.

These experiments demonstrate how initialization can affect the convergence process and final clustering solution.

