
Name: Vishal Prajapati Comapny: CODTECH IT SOLUTIONS ID:CT08DZU Domain: Data Science Duration: 17 Dec2024 - 17 Jan2025



Project Overview: Library Dataset Clustering and Analysis 

Output:



<img width="545" alt="Screenshot 2024-12-30 at 12 12 29 PM" src="https://github.com/user-attachments/assets/d00c7d37-b5cd-49a8-b29d-472570291829" />

<img width="468" alt="Screenshot 2024-12-30 at 12 12 56 PM" src="https://github.com/user-attachments/assets/3c7d0e14-fde7-432b-8fa9-27745577b2e6" />
<img width="468" alt="Screenshot 2024-12-30 at 12 15 24 PM" src="https://github.com/user-attachments/assets/2cf246f7-4137-4598-a25a-1e9bd872e588" />





This project involves clustering a library management dataset to identify patterns and insights into book genres, borrow frequency, ratings, and library branches. The aim is to group similar books or borrowing behaviors for better resource allocation, personalized recommendations, and operational efficiency. The project workflow is structured as follows:

1. Dataset Creation and Loading
If the dataset does not exist in the specified Google Drive folder, it generates a synthetic dataset containing the following attributes:
BookID: Unique identifier for each book.
Genre: Categorical variable representing the genre of the book.
Pages: Numerical attribute for the number of pages.
Ratings: Average user ratings (scale of 1-5).
BorrowFrequency: Frequency of borrowing.
LibraryBranch: Categorical variable for library locations.
The dataset is saved in CSV format for future use or loaded if it already exists.
2. Data Inspection
The dataset is examined for structure, types, and completeness using .head() and .info() methods to ensure data integrity before preprocessing.
3. Data Preprocessing
Selected features (Genre, Pages, Ratings, BorrowFrequency, LibraryBranch) are processed:
Numerical Features: Standardized using StandardScaler.
Categorical Features: Encoded with OneHotEncoder.
A combined matrix is created to prepare the data for clustering algorithms.
4. Optimal Number of Clusters
The Elbow Method is employed to determine the optimal number of clusters by plotting the inertia (sum of squared distances) against different cluster counts.
5. Clustering
K-Means Clustering is performed with the optimal cluster count.
Cluster labels are assigned to each book in the dataset, enabling segmentation.
6. Evaluation of Clustering
Clustering quality is assessed using:
Silhouette Score: Measures cohesion and separation.
Davies-Bouldin Index: Lower values indicate better clustering.
7. Visualization
Dimensionality reduction with PCA is applied to reduce the processed data to 2 dimensions for visualization.
Clusters are visualized using scatter plots, highlighting the grouping of books based on the reduced features.
Key Deliverables
Insights into the clustering of books based on genres, borrow patterns, and ratings.
Visual representations of cluster distributions.
Metrics evaluating clustering effectiveness.
Applications
Enhancing library inventory management.
Personalized book recommendations.
Resource optimization across library branches.
