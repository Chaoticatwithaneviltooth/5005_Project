# 5005_Project

## Project Title: Dimensionality Reduction and Clustering of AML RNA-seq Data Using Autoencoders

### Project Proposal 
This project aims to leverage autoencoders, a deep learning technique, for the dimensionality reduction of RNA-seq data from AML patients, facilitating the identification of inherent gene expression patterns and potential subtypes within the data through unsupervised clustering.

## Process

Utilize a deep learning autoencoder for dimensionality reduction of RNA-seq data from AML patients to a lower-dimensional space, facilitating the identification of inherent patterns or clusters within the data.

Steps to Complete the Project

**Day 1:** Project Setup and Data Preprocessing

Prepare your environment (e.g., Python with TensorFlow or PyTorch).
Preprocess the RNA-seq data (normalization, filtering).

**Day 2-3:** Implementing the Autoencoder

**Day 2:** Design a simple autoencoder architecture suitable for your dataset. The focus will be on creating a model that can compress the high-dimensional RNA-seq data to a lower-dimensional representation.

**Day 3:** Train the autoencoder on your RNA-seq data. This involves feeding the normalized gene expression data into the model, adjusting parameters as necessary to improve the learning process.

**Day 4:** Dimensionality Reduction and Data Visualization

Use the trained autoencoder to reduce the dimensionality of your RNA-seq data. Extract the encoder part of the network to get the compressed representation of your data.
Visualize the reduced data using PCA or t-SNE to observe any natural clustering or patterns.

**Day 5:** Clustering on Reduced Data

Apply a clustering algorithm (e.g., K-means, hierarchical clustering) to the lower-dimensional data to identify distinct groups of samples.
Analyze the clusters to see if they reveal any interesting patterns or potential subtypes within the AML samples.

**Day 6:** Biological Interpretation

Perform preliminary analysis to understand the biological significance of the clusters. This might involve identifying hallmark genes in each cluster and exploring their known associations with AML or related processes.

**Day 7:** Reporting and Future Directions

Compile your findings into a concise report or presentation. Highlight the methodology, the ML/DL models used, the results from the clustering, and any biological insights gained.
Suggest future directions for expanding the analysis, such as integrating additional datasets, exploring other ML/DL models, or conducting experimental validation.

# Dataset Access

- RNA Expression Array Data for Acute Myeloid Leukemia (183 patient samples) -> [https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE68833](url)

- Affymetrix Human Genome U133 Plus 2.0 Array -> [https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GPL570](url)

# Resources

- Preprocessing and Annotation of GEO Dataset -> [https://www.youtube.com/watch?v=9MqN06qCxGw](url)
- 
