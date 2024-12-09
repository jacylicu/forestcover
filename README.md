Forest Cover Classification


Introduction
Problem

This project classifies forest cover, primary species of trees present, found in the Roosevelt National Forest in Colorado based on several attributes such as shadow coverage, soil type, local topography, and distance to landmarks. Both supervised and unsupervised learning methods are used. Due to the size of the data >500,000, a subset of the data is used to unsupervised learning.

Columns and explanations:

- Elevation: Height above sea level in meters.
- Aspect: Direction the slope faces, measured in degrees from 0 to 360.
- Slope: Steepness of the terrain, measured in degrees.
- Horizontal_Distance_To_Hydrology: Distance to the nearest water source, like a stream or lake, measured in meters.
- Vertical_Distance_To_Hydrology: Height difference between the point and the nearest water source, measured in meters.
- Horizontal_Distance_To_Roadways: Distance to the nearest road, measured in meters.
- Hillshade_9am/Noon/3pm: Amount of shade at the point at different times of the day, ranging from 0 (fully shaded) to 255 (fully lit).
- Horizontal_Distance_To_Fire_Points: Distance to the nearest known fire location, measured in meters.
- Wilderness_Area1-4: Binary indicators representing different designated wilderness areas (1 if true, 0 if false).
- Soil_Type1-40: Binary indicators for specific soil types based on predefined categories


Cover Type

1. Deciduous Forests
2. Coniferous Forests (Evergreens)
3. Mixed Forests: A combination of deciduous and coniferous trees.
4. Tropical Rainforests
5. Boreal Forests (Taiga)
6. Temperate Forests
7. Mangrove Forests
Data Source

This dataset is part of the UCI Machine Learning Repository. The original database owners are Jock A. Blackard, Dr. Denis J. Dean, and Dr. Charles W. Anderson of the Remote Sensing and GIS Program at Colorado State University.

Data be downloaded at: https://www.kaggle.com/datasets/uciml/forest-cover-type-dataset

Outline

Importing libraries and data
Exploratory Data Analysis (EDA):
Inspect data distribution and values
Visualize data distribution and values
Clipping outliers
Finding correlations (apply PCA to address the problem)
Data transformation: Using StandardScaler to scale numerical data
Data transformation: Run PCA (principle component analysis) on the data
Supervised Learning Models: Random Forest and Logistics Regression
Unsupervised Learning Models: KMeans, DBSCAN (Density Based Clustering) and Hierarchical Clustering
Comparison based on accuracy score, silhouette score, ARI score, and run time
Conclusion
