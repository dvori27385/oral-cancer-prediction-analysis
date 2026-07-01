# Oral Cancer Prediction & Analysis

This project focuses on predicting oral cancer development based on clinical and personal risk factors. It utilizes data mining techniques to identify significant attributes and build classification models.

## 📊 Project Methodology (KDD Process)

The project followed the standard KDD stages:
- **Data Collection & Cleaning**: Handled duplicate records to ensure data integrity.
![Data Cleaning](images/data-cleaning-duplicates.png.png)

- **Data Transformation**: Performed discretization on the 'Age' attribute to improve model performance.
![Age Discretization](images/age-discretization.png)

- **Attribute Selection**: Applied Information Gain analysis to identify the most predictive features.
![Data Distribution](images/data-distribution-weka.png)
![Attribute Selection](images/attribute-selection-weka.png)

## 🤖 Models & Classification

### 1. ID3 Algorithm
![ID3 Model](images/id3-decision-tree-model.png)
![ID3 Performance](images/id3-performance-metrics.png)

### 2. J48 Algorithm (C4.5)
![J48 Performance](images/j48-performance-metrics.png)
![J48 Tree](images/j48-decision-tree-visualization.png)

## 📈 Conclusion & Analysis
The models highlight that 'Country' and 'Age' are significant predictors, although clinical features showed a moderate correlation in this specific dataset. 

## 📄 Full Report
For the complete technical documentation, you can refer to the [project PDF](MMN21...pdf).
