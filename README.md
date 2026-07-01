# Data Mining Project: Oral Cancer Analysis (Full KDD Process)

This repository contains a comprehensive data mining project analyzing oral cancer risk factors. The project was conducted in two phases, covering the full Knowledge Discovery in Databases (KDD) lifecycle using the WEKA environment.

---

## 🟢 Part 1: Data Preprocessing & Classification
*Focus: Data cleaning, feature selection, and predictive modeling using decision trees.*

- **Data Preprocessing**: Handled duplicate records and discretized continuous variables like 'Age'.
- **Classification Models**: Implemented ID3 and J48 Decision Trees.
- **Key Finding**: Clinical features showed weak predictive power (~50% accuracy), highlighting the limitations of questionnaire-based medical data.

**J48 Decision Tree Visualization:**
![J48 Tree](images/j48-decision-tree-visualization.png)

📄 **[View Full Part 1 Report (Maman 21)](MMN21...pdf)** 

---

## 🔵 Part 2: Advanced Analysis & Unsupervised Learning
*Focus: Association rules, Clustering, and Neural Networks.*

### 1. Association Rules (Apriori)
Used to identify behavioral patterns linked to health outcomes. 
- **Key Insight**: Identified strong associations between risk behaviors (smoking, alcohol) and the target variable.
![Apriori Rules](mmn22/m22-apriori-best-rules.png)

### 2. Clustering (K-Means)
Attempted to group patients without target labels. The algorithm formed two clusters primarily based on dietary habits, but failed to separate patients based on their cancer diagnosis.
![K-Means Clusters](mmn22/m22-kmeans-cluster-visualization.png)

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
