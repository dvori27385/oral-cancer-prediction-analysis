# Oral Cancer Prediction & Analysis (Full Data Mining Project)

This repository contains a comprehensive data mining project analyzing oral cancer risk factors. The project was conducted in two phases (Maman 21 & Maman 22), covering the full Knowledge Discovery in Databases (KDD) lifecycle using the WEKA environment.

---

## 🟢 Part 1: Data Preprocessing & Classification (Maman 21)

### 📊 Project Methodology (KDD Process)
- **Data Collection & Cleaning**: Handled duplicate records to ensure data integrity.
![Data Cleaning](images/data-cleaning-duplicates.png.png)

- **Data Transformation**: Performed discretization on the 'Age' attribute to improve model performance.
![Age Discretization](images/age-discretization.png)

- **Attribute Selection**: Applied Information Gain analysis to identify the most predictive features.
![Data Distribution](images/data-distribution-weka.png)
![Attribute Selection](images/attribute-selection-weka.png)

### 🤖 Models & Classification
#### 1. ID3 Algorithm
![ID3 Model](images/id3-decision-tree-model.png)
![ID3 Performance](images/id3-performance-metrics.png)

#### 2. J48 Algorithm (C4.5)
![J48 Performance](images/j48-performance-metrics.png)
![J48 Tree](images/j48-decision-tree-visualization.png)

📄 **[View Full Part 1 Report (Maman 21)](MMN21...pdf)** 

---

## 🔵 Part 2: Advanced Analysis & Unsupervised Learning (Maman 22)

### 1. Association Rules (Apriori)
Used to identify behavioral patterns linked to health outcomes. 
- **Key Insight**: Identified strong associations between risk behaviors (smoking, alcohol) and the target variable.
![Apriori Large Itemsets](mmn22/m22-apriori-large-itemsets.jpg.png)
![Apriori Rules](mmn22/m22-apriori-best-rules.png)

### 2. Clustering (K-Means)
Attempted to group patients without target labels. The algorithm formed two clusters primarily based on dietary habits, but failed to separate patients based on their cancer diagnosis.
![K-Means Clusters](mmn22/m22-kmeans-cluster-visualization.png)
![K-Means Centroids](mmn22/m22-kmeans-cluster-centroids.jpg.png)

### 3. Neural Networks (MLP)
Implemented a Multi-Layer Perceptron (3 layers, 10 hidden neurons) to capture complex non-linear relationships.
- **Results**: Accuracy remained around 49.8%, and the error convergence was slow, confirming the inherent noise and limitations in the dataset.
![Neural Network Architecture](mmn22/m22-nural-network-architecture.jpg.png)
![Error Convergence](mmn22/m22-neural-network-convergence.png)

📄 **[View Full Part 2 Report (Maman 22)](MMN22.pdf)** 

---

## 🏁 Final Conclusion
Across all models—supervised and unsupervised—the algorithms performed correctly, but the accuracy consistently hovered around 50%. This project demonstrates a crucial data science principle: **data quality dictates model quality**. Predicting clinical diagnoses requires robust medical data (e.g., lab tests, genetics) rather than just lifestyle surveys.

## 🛠️ Technical Stack
- **Tools**: WEKA, Microsoft Excel.
- **Algorithms**: ID3, J48, Apriori, K-Means, Multi-Layer Perceptron.
- **Dataset**: Processed patient records (`MMN21.csv`).
