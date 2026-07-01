# Oral Cancer Prediction & Analysis

This project focuses on predicting oral cancer development based on clinical and personal risk factors. It utilizes data mining techniques to identify significant attributes and build classification models to aid in early diagnosis.

## 📊 Project Methodology (KDD Process)

The project followed the standard Knowledge Discovery in Databases (KDD) stages:
- **Data Collection & Cleaning**: Handled duplicate records to ensure data integrity and statistical accuracy.
- **Data Transformation**: Performed discretization on the 'Age' attribute to improve model performance and reduce noise.
- **Attribute Selection**: Applied Information Gain analysis to identify the most predictive features, such as 'Country' and 'Age'.

![Data Distribution](images/data-distribution-weka.png)

## 🤖 Models & Classification

I experimented with two primary classification algorithms using the WEKA platform:

### 1. ID3 Algorithm
A classic decision tree approach that uses Information Gain for node splitting.
![ID3 Decision Tree](images/id3-decision-tree-model.png)

### 2. J48 Algorithm (C4.5)
An improved version of ID3, utilizing Gain Ratio and post-pruning to prevent overfitting and improve model robustness.
![J48 Performance Metrics](images/j48-performance-metrics.png)
![J48 Decision Tree](images/j48-decision-tree-visualization.png)

## 📈 Conclusion & Analysis
Both models achieved an accuracy of approximately 50%, suggesting that the selected clinical features in this specific dataset have a weak correlation with the diagnosis. This project highlights the importance of data quality and the challenges of feature selection in medical diagnosis tasks.

## 📄 Full Report
For the complete technical documentation, including pseudo-code and detailed analysis, you can refer to the [project PDF](reports/YOUR_PDF_NAME.pdf).
