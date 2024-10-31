# "Clustering and Analysis of U.S. Traffic Accident Patterns"

This project analyzes traffic accident data across various U.S. states to identify patterns and inform potential policy interventions. The analysis includes data exploration, correlation analysis, dimensionality reduction with PCA, and clustering using KMeans.

## How to run the project:
For running the ipynb file, using google colab would be enough.

## Project Structure

- **1. Raw Data Files**: This project uses traffic accident data from the National Highway Traffic Safety Administration and the National Association of Insurance Commissioners, compiled by FiveThirtyEight under the CC-BY4.0 license. The data is located in the `datasets/road-accidents.csv` file.
  
- **2. Data Overview**: We begin by loading the data and exploring its structure to understand the features available for analysis.

- **3. Data Summary**: Summary statistics and visualizations, including histograms and scatter plots, provide an overview of the distribution and relationships within the data.

- **4. Feature Correlation**: The Pearson correlation matrix quantifies relationships between variables, helping to identify associations with fatal accident rates.

- **5. Multivariate Linear Regression**: A regression model quantifies feature associations with the target variable, `drvr_fatl_col_bmiles`, while adjusting for confounding factors.

- **6. Dimensionality Reduction**: Principal Component Analysis (PCA) reduces data dimensionality, allowing us to visualize state groupings based on similarities.

- **7. Clustering**: We apply KMeans clustering to identify groups of states with similar accident profiles, using both PCA and scree plots to guide the number of clusters.

- **8. Cluster Analysis**: Clusters are visualized and analyzed to understand differences in traffic accident patterns, focusing on `perc_fatl_speed`, `perc_fatl_alcohol`, and `perc_fatl_1st_time`.

- **9. Accident Totals by Cluster**: Using additional data on miles driven, we compute and visualize total accident counts by cluster, helping prioritize interventions.

## Project Requirements

The following Python packages are required:
- `pandas`
- `seaborn`
- `matplotlib`
- `scikit-learn`

