# Conformational Analysis Using Machine Learning

This repository contains code for analyzing molecular dynamics (MD) simulation data using machine learning techniques. The workflow includes feature extraction, dimensionality reduction, clustering, classification, and the selection of a representative conformation for each cluster using the centroid method.

**Note:** The specific protein analyzed in this project is not disclosed for confidentiality reasons. Additionally, this research is ongoing, and updates may be made in the future.

## Project Workflow

- **Feature Extraction**:
  - Extracts relevant features from MD simulation data, such as RMSD,RG,hydrogen bonds, SASA, and backbone distance matrices.

- **Dimensionality Reduction**:
  - Uses Principal Component Analysis (PCA) to reduce the dimensionality of the extracted features, ensuring that the key variances in the data are retained.

- **Clustering**:
  - Applies clustering algorithms (such as K-means) to group similar conformations based on reduced features.

- **Classification**:
  - Classifies the clusters using machine learning algorithms, evaluating the results using accuracy and cross-validation.

- **Representative Conformation Selection**:
  - For each cluster, a representative conformation is selected using the centroid method to best represent the cluster.

## How to Use the Code

1. **Prerequisites**:
    - Install Python and Jupyter Notebook.
    - Install necessary Python libraries:
    ```bash
    pip install numpy pandas scikit-learn matplotlib mdtraj 
    ```

2. **Running the Code**:
    - Open the provided `.ipynb` notebook in Jupyter Notebook.
    - Load your own MD simulation data or follow the example in the notebook.
    - Run through the steps of feature extraction, PCA, clustering, and classification.

3. **Customization**:
    - The code is modular, allowing you to adjust feature extraction, PCA parameters, or clustering techniques depending on your dataset and research needs.

## Future Updates

- The project is still in progress. Additional features, refinements in clustering methods, and further analysis will be added as the research continues.

## Disclaimer

This code is part of ongoing research and is provided "as is." The research involves the analysis of a specific protein, but its name and details are not included in this repository.
