# Customer Segmentation with K-Means

This repository contains a practical data science project focused on customer segmentation using unsupervised machine learning.

The project applies an end-to-end workflow in Python: data loading, exploratory analysis, data cleaning, feature engineering, feature scaling, K-Means clustering, model evaluation and business interpretation of the resulting customer groups.

## Main objectives

- Clean and prepare customer-level data for modelling
- Handle missing values and inconsistent numerical fields
- Convert categorical variables using one-hot encoding
- Engineer behavioural features such as reminders per year
- Apply K-Means clustering for customer segmentation
- Use elbow and silhouette analysis to support the choice of clusters
- Interpret customer clusters from a business perspective
- Export customer-level cluster labels and cluster summary tables

## Repository structure

```text
customer-segmentation-kmeans/
├── customer_segmentation_kmeans.ipynb
├── data/
│   └── input/
│       └── raw_database.csv
├── reports/
│   ├── raw_database_report.html
│   └── modified_database_report.html
├── outputs/
│   ├── customer_clusters.csv
│   └── cluster_summary.csv
└── requirements.txt
```

## How to run the notebook

Install the required Python libraries:

```bash
pip install -r requirements.txt
```

Then open the notebook:

```bash
jupyter notebook customer_segmentation_kmeans.ipynb
```

The notebook uses relative paths, so it does not require Google Drive or Google Colab-specific folders.

## Methodology

The analysis follows these steps:

1. Load the raw customer dataset.
2. Inspect data types, missing values and descriptive statistics.
3. Clean missing suspension requests and convert monetary fields.
4. Replace negative values in naturally non-negative features.
5. One-hot encode the `supply` variable.
6. Create a new feature measuring reminders per year.
7. Scale the selected features.
8. Use elbow and silhouette analysis to compare different numbers of clusters.
9. Fit a final K-Means model.
10. Profile and interpret each customer cluster.
11. Export customer cluster labels and summary tables.

## Technologies used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook

## Academic / training context

This project was developed as part of a data science training exercise. It is intended as a practical example of customer analytics, clustering and business-oriented machine learning.
