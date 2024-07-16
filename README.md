# IST-with-GM-clustering

## Dataset

1. <b> IST_corrected: </b>
   The original dataset for International Stroke Trial database available at https://datashare.ed.ac.uk/handle/10283/124

2. <b> Cleaned_data: </b>
   Resulting dataset after data cleaning

3. <b> Clustered_GM: </b>
   Resulting dataset for visualization after applying Gaussian Mixture clustering with parameters number of clusters = 4 and covariance type = 'spherical'

## Notebooks

1. <b>Data Cleaning: </b>
   The notebook focuses on transforming datasets to facilitate utilization with clustering algorithms and data analysis tools while filtering out patients who survived beyond fourteen days post-hospital discharge period by selecting 'Y' from the DALIVE variable, resulting in a reduced number count from the initial nineteen thousand four hundred thirty-four patients down ten thousand one hundred thirty-eight patients. The process includes deleting entries with incomplete data, standardizing data to get uniform format, and addressing encoding issues.

2. <b>Clustering_v5: </b>
   Includes parameter tuning to find the best parameter among the specified range of parameter values. The top performing parameters are then used and applied with clustering algorithms which are BIRCH, Agglomerative, and Gausian Mixture clustering algoritms. Silhouette, DBI, and Calinski Harabasz scores are then used to measure the best performing algorithm among the mentioned clustering algortims for the specified dataset.

3. <b>GM_Clustered_Data_Visualization: </b>
   Data visualization of the dataset produced from clustering the Cleaned_data with Gaussian Mixture Algorithm. Pyplot and seaborn are used for data visualization.
