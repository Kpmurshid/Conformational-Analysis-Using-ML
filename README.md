# Conformational Analysis Using Machine Learning

This repository contains code for analyzing molecular dynamics (MD) simulation data using machine learning techniques. The workflow includes feature extraction, dimensionality reduction, clustering, classification, and the selection of a representative conformation for each cluster using the centroid method. Additionally, validation is performed using DSSP to confirm secondary structure assignments.

**Note:** The specific protein analyzed in this project is not disclosed for confidentiality reasons. Additionally, this research is ongoing, and updates may be made in the future.

## Project Workflow

- **Feature Extraction**:
  - Extracts relevant features from MD simulation data, such as RMSD, radius of gyration (Rg), hydrogen bonds, SASA, and backbone distance matrices.

- **Dimensionality Reduction**:
  - Utilizes an autoencoder, a deep learning-based approach, to reduce the dimensionality of the extracted features. The autoencoder learns a compact representation of the data while preserving essential features.

- **Clustering**:
  - Applies clustering algorithms (such as K-means) to group similar conformations based on reduced features from the autoencoder.

- **Classification**:
  - Classifies the clusters using machine learning algorithms and evaluates the results through accuracy and cross-validation.

- **Representative Conformation Selection**:
  - For each cluster, a representative conformation is selected using the centroid method to best represent the cluster.

- **Validation Using DSSP**:
  - The secondary structure of representative conformations is validated using DSSP (Define Secondary Structure of Proteins) to confirm structural consistency with the original data.

## How to Use the Code

1. **Prerequisites**:
    - Install Python and Jupyter Notebook.
    - Install necessary Python libraries:
    ```bash
    pip install numpy pandas scikit-learn matplotlib mdtraj tensorflow keras
    ```

2. **Running the Code**:
    - Open the provided `.ipynb` notebook in Jupyter Notebook.
    - Load your own MD simulation data or follow the example in the notebook.
    - Run through the steps of feature extraction, dimensionality reduction using the autoencoder, clustering, classification, and DSSP validation.

3. **Customization**:
    - The code is modular, allowing you to adjust feature extraction, autoencoder architecture, or clustering techniques depending on your dataset and research needs.

