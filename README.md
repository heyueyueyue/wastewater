# Introduction
This repository contains a comprehensive Python script designed for microbial data analysis. The script includes functionalities for retrieving microbial classification information, detecting suspected microorganisms, analyzing microbial abundances, calculating diversity indices, performing similarity analysis, conducting cluster analysis, and executing Principal Coordinates Analysis (PCoA) and Principal Component Analysis (PCA).

# Data
The analysis relies on various CSV files that contain microbial taxonomic data and abundance estimates. Key data files include:

nodes.dmp: Contains hierarchical taxonomic information.
names.dmp: Provides names associated with tax IDs.
HTPMs.csv: Contains microbial Tax IDs and Latin names.
oth.csv: Includes data for detecting suspected microorganisms.
cluster.csv: Used for cluster analysis.
apr.csv: Contains data for PCoA and PCA analysis.

# Code
The code is written in Python and requires the following libraries:

pandas: For data manipulation and analysis.
numpy: For numerical operations.
scipy: For clustering and distance calculations.
matplotlib: For data visualization.
skbio: For statistical ordination.
sklearn: For machine learning and preprocessing.
To install the required libraries, run:

pip install pandas numpy scipy matplotlib scikit-bio scikit-learn
Preparation
Ensure the following files are available in your working directory:

nodes.dmp
names.dmp
HTPMs.csv
oth.csv
cluster.csv
apr.csv
Make sure the paths to these files are correctly specified in the code.

# Run
To execute the analysis, run the following command in your terminal or command prompt:

python your_script_name.py
The script processes the data through several stages:

Microbial Classification Information Retrieval: Reads taxonomic data files and adds classification information to the microbial data.
Detection of Suspected Microorganisms: Analyzes input data for specific dates and marks the presence of microorganisms.
Top 5 Dominant Microbial Abundances: Calculates and saves the top microbial abundances for specified scenarios.
Diversity Indices Calculation: Computes various diversity indices based on microbial abundance data.
Similarity Analysis: Compares microbial data between two datasets and calculates similarity metrics.
Cluster Analysis: Performs hierarchical clustering and visualizes the results using a dendrogram.
PCoA and PCA: Conducts ordination analyses to visualize microbial community structure and identify key variables.

# Code Structure
The main functionalities in the code are organized as follows:

1.1 - Find Microbial Classification Information: Reads taxonomic files and retrieves classification data.
1.2 - Detection of Suspected Input Microorganisms: Processes input data to identify suspected microorganisms based on date.
1.3 - Top 5 Dominant Microbial Abundances: Analyzes microbial abundances for different scenarios.
2 - Calculate Diversity Indices: Computes diversity metrics from abundance data.
3.1 - Calculate Similarity: Measures similarity between two datasets.
3.2 - Cluster Analysis: Performs clustering on microbial data and visualizes the results.
4 - PCoA and PCA: Executes ordination analyses to explore microbial community structure.

# License
The code and data are released under the MIT License.
