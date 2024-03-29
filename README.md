# 5005_Project

## Project Title: Leveraging Deep Learning for Subtype Identification and Biomarker Discovery in AML

### Project Proposal 
This project aims to utilize advanced deep learning techniques to analyze RNA-seq data from AML patients, identifying distinct molecular subtypes and key biomarkers, thereby facilitating the development of personalized therapeutic strategies.

*** (The following text below is not confimred just an idea to follow)
### Subtype Identification and Characterization with Deep Learning
- Autoencoders: An unsupervised deep learning approach, autoencoders can reduce the dimensionality of RNA-seq data, capturing the most salient features in a lower-dimensional space. The reduced feature set can then be used for clustering, making it easier to identify distinct AML subtypes.
- Clustering on Embedded Space: After dimensionality reduction, deep learning-based clustering techniques, such as deep embedded clustering, can be applied to the encoded representations to identify distinct patient groups representing different AML subtypes.
- Convolutional Neural Networks (CNNs): Although traditionally used for image data, CNNs can also be applied to sequence and expression data, capturing local patterns within the data that might signify subtype-specific expression profiles.
### Biomarker Discovery for AML with Deep Learning
- Feature Importance: Deep learning models, especially those with attention mechanisms, can highlight which genes (features) are most informative for subtype classification. These key features can serve as potential biomarkers.
- Supervised Learning: Once subtypes are established, supervised deep learning models can be trained to predict the subtype based on gene expression, with the model learning to focus on genes that best distinguish between subtypes. Techniques like SHAP (SHapley Additive exPlanations) and LIME (Local Interpretable Model-agnostic Explanations) can then be used to interpret these models and identify the most important features (genes) used for classification.

# Dataset Access

- RNA Expression Array Data for Acute Myeloid Leukemia (183 patient samples) -> [https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE68833](url)

- Affymetrix Human Genome U133 Plus 2.0 Array -> [https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GPL570](url)

# Resources

- Preprocessing and Annotation of GEO Dataset -> [https://www.youtube.com/watch?v=9MqN06qCxGw](url)
- 
