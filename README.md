# Master Thesis: Predicting Dementia Types Using Machine Learning on Aggregate Images

### Overview
Dementia is a rapidly growing public health concern, characterised by the accumulation of misfolded protein aggregates in the brain. The morphological differences between these aggregates have been suggested as a potential parameter to diagnose different types of dementia. This project aims to establish a machine learning pipeline to predict four types of dementia: Parkinson’s Disease (PD), Dementia with Lewy Bodies (DLB), Frontotemporal Dementia (FTD), and Alzheimer’s Disease (AD). It also seeks to differentiate the morphological features of aggregates specific to these diseases.

### Methods:
- **Feature Extraction**: Two methods were employed for feature extraction from single aggregate images:
  1. Convolutional Autoencoder (CAE)
  2. Computational shape measurements using the IMEA package
- **Dimensionality Reduction**: Uniform Manifold Approximation and Projection (UMAP) was used to reduce dimensionality of extracted features.
- **Clustering and Classification**: K-Means clustering was applied, followed by Dirichlet regression to identify disease-specific clusters. Various classifiers, including logistic regression, support vector machine, random forest and XGBoost were evaluated for dementia type prediction.

<img src="https://github.com/user-attachments/assets/a06a3cef-a935-4ed5-b15c-6a8cef943ec8" alt="CompEpi" width="800"/>

### Results:
Random forest demonstrated the best balance between performance and reliability, achieving a weighted average AUC of 0.64 for the CAE pipeline and 0.68 for the IMEA pipeline. The results provide a **foundational framework for developing a scalable, high-throughput diagnostic tool using aggregate morphology**. The identified clusters validate morphological distinctions of protein aggregates specific to different dementia types.

<img src="https://github.com/user-attachments/assets/b84a016a-c496-4e48-95f4-cc9d2e635da8" alt="CompEpi" width="800"/>

### Usage
This repository contains the framework for establishing the prediction pipeline. However, the relevant code for this project is reserved for lab use. For more details, please contact the Ye Lab at Imperial College London.

### Acknowledgements
This work was supervised by Dr. Yu Ye at the Ye Lab, Imperial College London. Special thanks to Dr. Michael Morten and Hailey Gu for their insights and technical support, and the support team for their assistance in developing the scripts used in this study.
