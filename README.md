## Generic Recommendation System
## Introduction
 This project aims to develop a versatile recommendation system that can be applied to any dataset adhering to a standardized format. The system utilizes content-based clustering algorithms and natural language processing (NLP) to provide personalized recommendations for movies, TV shows, universities, or other items based on user preferences and item characteristics.

## Problem Statement
 The project addresses the challenge of recommendation fatigue, where users struggle to make informed decisions due to an overwhelming number of options. Our recommendation system overcomes this challenge by providing personalized suggestions tailored to each user's interests.

## Data
 The project utilizes two datasets:

 Netflix Dataset: This dataset consists of 12 attributes and 7787 rows, encompassing information about various movies and TV shows.

 University Information Dataset: This dataset includes various attributes related to universities, such as tuition fees, acceptance rates, and location.

![Image 11-21-23 at 8 40 PM](https://github.com/shahjahnavi/Generic_clustering_system_for_any_data/assets/138523298/a6bab648-f2b5-4584-9f18-dcd9ee35892d)

![Image 11-21-23 at 8 41 PM](https://github.com/shahjahnavi/Generic_clustering_system_for_any_data/assets/138523298/baf73af2-9daa-4877-8d1d-558724cfef63)



## Data Preparation and Exploratory Data Analysis (EDA)
 Prior to model development, the data underwent thorough data preparation and EDA steps:

 Data Comprehension: A comprehensive understanding of the data was gained by analyzing eight attributes on both sides, including a mix of structured and unstructured data features.

 Data Cleaning: To ensure high-quality recommendations, extensive data cleaning was performed to address any inconsistencies or anomalies in the data.

## Model
 The recommendation system employs a K-means clustering algorithm, which is a popular unsupervised learning technique for grouping similar data points into clusters.

 Feature Selection: Principal component analysis (PCA) was used to identify the most relevant features for clustering, reducing the dimensionality of the data to 4000 attributes.

 Determining Optimal Cluster Number: Various methods, including the elbow method and silhouette analysis, were employed to determine the optimal number of clusters, resulting in 6 clusters for the Netflix dataset and 12 clusters for the university dataset.

 Hierarchical Clustering: Hierarchical clustering was further applied to refine the clustering results, leading to a final cluster count of 12 for both datasets.

Cosine Similarity for Contextual Similarity
 The recommendation system utilizes a cosine similarity function to determine contextual similarity between items, providing a generic and adaptable solution. The cosine function measures the similarity between two vectors by calculating the dot product of the vectors divided by the magnitude of each vector.

![Image 11-21-23 at 8 41 PM](https://github.com/shahjahnavi/Generic_clustering_system_for_any_data/assets/138523298/86ac50f6-a567-4566-abbb-c33bc70ff721)

![Image 11-21-23 at 8 42 PM](https://github.com/shahjahnavi/Generic_clustering_system_for_any_data/assets/138523298/785fd1c4-781c-43ff-845f-1244119d3a6e)


## Findings and Evaluation
 Recommendations: The recommendation system successfully generated recommendations for movies, TV shows, and universities based on the respective datasets.

 Comparison with Manual Recommendations: Upon comparing the system's recommendations to manual recommendations, it was found that the system prioritized certain attributes, such as description and tuition fees, more than others.

 Visualization: A Directed Acyclic Graph (DAG) was generated using a NetworkX layer to visualize the clustering algorithm.

 Centroid Improvement: Hierarchical clustering enhanced the centroids, leading to reduced distances between data points and improved algorithm performance.


![Image 11-21-23 at 8 42 PM](https://github.com/shahjahnavi/Generic_clustering_system_for_any_data/assets/138523298/43590219-788b-41c4-9b47-056463fcb920)

![Image 11-21-23 at 8 43 PM](https://github.com/shahjahnavi/Generic_clustering_system_for_any_data/assets/138523298/5bca218a-d920-4b82-9110-b531ce20dc43)


## Conclusions and Future Scope
 Generic Recommendation System: The project successfully developed a generic recommendation system capable of handling any dataset adhering to a standardized format.

 Regularized Format Limitations: The system's performance was somewhat constrained by the limitations of the regularized data format.

 Data Format Impact: The data format influenced the generality of the recommendations, with stronger and more trained algorithms potentially improving the results.

Future Work: The project aims to explore transformer-based methodologies, such as GPT and BERT, to handle unstructured data and enhance recommendation accuracy.

Multi-Dataset Training: The project intends to further develop the system by training it on multiple datasets simultaneously to increase training points.

Feature Selection and Filtering: Advanced feature selection and filtering techniques will be investigated to accelerate the production of more accurate results.


## The following libraries are used in the code:

pandas: Data analysis and manipulation library
numpy: Numerical operations library
datetime: Date and time manipulation library
warnings: Library for controlling warning messages
nltk: Natural language processing (NLP) library
wordcloud: Word cloud visualization library
re: Regular expression library
string: String manipulation library
unicodedata: Unicode character handling library
sklearn.feature_extraction.text: Text feature extraction library
sklearn.decomposition: Dimensionality reduction library
WordNetLemmatizer: Word lemmatization library
sklearn.cluster: Clustering algorithm library
sklearn.metrics: Model evaluation metrics library
scipy.cluster.hierarchy: Hierarchical clustering library
networkx: Network graph analysis library
plotly: Visualization library
matplotlib: Visualization library
seaborn: Statistical data visualization library
