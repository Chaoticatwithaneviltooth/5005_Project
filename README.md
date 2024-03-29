# 5005_Project

## Project Title: Leveraging Deep Learning for Subtype Identification and Biomarker Discovery in AML

### Project Proposal 
This project aims to utilize advanced deep learning techniques to analyze RNA-seq data from AML patients, identifying distinct molecular subtypes and key biomarkers, thereby facilitating the development of personalized therapeutic strategies.

#### Step 1: Data Preparation
- Collect RNA-seq Data: Obtain RNA-seq datasets for AML patients. Public databases like NCBI's GEO can be a good source. Ensure the data is labeled if your aim includes supervised learning tasks.
- Preprocessing: Normalize the RNA-seq data to make gene expression levels comparable across samples. Convert the gene expression matrix into a format that mimics a 'text' document, where each gene can be considered a 'word' and each sample a 'document'. High expression genes might be repeated more times to reflect their 'importance', akin to word frequencies in text.
#### Step 2: Basic NLP Techniques
- Tokenization and Vectorization: Use a simple bag-of-words (BoW) model to convert your preprocessed 'documents' into vectors. Each unique gene represents a unique token in the BoW model. Python's sklearn.feature_extraction.text.CountVectorizer can be repurposed for this task.
- TF-IDF Transformation: Apply Term Frequency-Inverse Document Frequency (TF-IDF) transformation to weigh the genes in your vectors, highlighting genes that are important in specific samples but not common across all samples. Use sklearn.feature_extraction.text.TfidfTransformer.
#### Step 3: Clustering for Subtype Identification
- K-means Clustering: With vectors representing your samples, apply K-means clustering to group samples based on their gene expression profiles. The sklearn.cluster.KMeans class can be used for this purpose. Determine the optimal number of clusters (k) using the elbow method or silhouette scores, representing potential AML subtypes.
Interpretation: Analyze the clustering results to characterize each cluster. Look at the most distinctive genes (highest TF-IDF scores) in each cluster to start identifying potential biomarkers.
#### Step 4: Biomarker Identification
- Feature Importance: Within each cluster, identify genes that significantly differ from the rest. These are your potential biomarkers. Simple statistical tests or even manual inspection of the top TF-IDF scored genes can provide initial insights.
#### Step 5: Building a Prediction Model
- Supervised Learning with Logistic Regression: For a beginner-friendly model, use logistic regression to predict AML subtypes based on the expression levels of identified biomarkers. This approach is straightforward and interpretable. Split your data into training and testing sets to evaluate the model's performance.
- Evaluation: Use metrics such as accuracy, precision, recall, and F1 score to assess your model. sklearn.metrics provides these functions.
#### Step 6: Documentation and Reporting
- Document Your Process: Clearly document each step, including data preprocessing decisions, model selection rationale, and analysis of results. Jupyter Notebooks can be an excellent tool for this purpose.
- Prepare a Report: Summarize your findings, methodologies, challenges faced, and potential implications of your work. Highlight any interesting biomarkers identified and discuss how the identified subtypes could influence treatment strategies.
#### Tools and Libraries
Python will be your primary tool, with heavy reliance on libraries such as Pandas (for data manipulation), Scikit-learn (for ML tasks), and Matplotlib/Seaborn (for visualization).
#### Conclusion
This project offers a foundational approach to applying NLP concepts to RNA-seq data analysis. While it simplifies many aspects of bioinformatics and NLP to fit a beginner-friendly profile, it can serve as a stepping stone towards more complex analyses and the use of advanced models, like deep learning, for even richer insights.

# Dataset Access

- RNA Expression Array Data for Acute Myeloid Leukemia (183 patient samples) -> [https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE68833](url)

- Affymetrix Human Genome U133 Plus 2.0 Array -> [https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GPL570](url)

# Resources

- Preprocessing and Annotation of GEO Dataset -> [https://www.youtube.com/watch?v=9MqN06qCxGw](url)
- 
