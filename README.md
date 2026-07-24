Breast Cancer Classification using K-Nearest Neighbors (KNN)
Author: Pranhavee Tyagi

Registration Number: 23BCE11740

Application Number: IN26009567

Batch Number: 2B

Email ID: pranhavee.23bce11740@vitbhopal.ac.in

Objective
The objective of this project is to build a K-Nearest Neighbors (KNN) classification model (
k
=
5
) to accurately classify breast tumors as Malignant (M) or Benign (B) based on diagnostic measurements.

Dataset Link
Kaggle: Breast Cancer Wisconsin Diagnostic Dataset
Libraries Used
pandas
numpy
matplotlib
seaborn
scikit-learn
kaggle
Methodology
Data Understanding: Identified numerical features and target variable (diagnosis), inspecting data types and distributions.
Data Preprocessing:
Dropped unnecessary columns (id and Unnamed: 32).
Encoded target variable diagnosis (M: 1, B: 0).
Split dataset into 80% training and 20% testing sets using stratified sampling.
Standardized features using StandardScaler to equalize feature contributions across distance metrics.
Model Development: Trained a KNeighborsClassifier with 
k
=
5
 on the scaled training features.
Model Evaluation: Evaluated the model using Accuracy, Precision, Recall, F1-Score, and a Confusion Matrix heatmap.
Results
Accuracy: 95.61%
Precision: 97.44%
Recall: 90.48%
F1-Score: 0.9383
Conclusion
The KNN model (
k
=
5
) successfully classifies tumor samples with 95.61% accuracy. Feature scaling with StandardScaler is essential to prevent distance dominance by large-magnitude features. While highly effective for small diagnostic datasets, KNN's primary limitation is its high memory footprint and query latency when scaling to larger datasets.
