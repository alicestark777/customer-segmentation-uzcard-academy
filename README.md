# Customer Segmentation with K-Means and DBSCAN

## Overview
This project explores customer segmentation for a banking context using Python, pandas, scikit-learn, and PostgreSQL. The notebook prepares customer-level features from multiple data tables, applies K-Means and DBSCAN, compares the resulting clusters, and profiles the segments to discuss possible business actions.

## Files
- `feature_kmeans_dbscan_clean.ipynb` — analysis notebook. Database credentials are read from environment variables; notebook outputs have been cleared before sharing.
- `customer_segmentation_v3.pptx` — presentation describing the methodology, findings, model comparison, and potential business implications.

## Methods and workflow
1. Load source tables from PostgreSQL or local CSV files.
2. Build customer-level features across balances, revenue, product usage, transactions, and customer lifecycle.
3. Prepare numeric features using outlier treatment and scaling.
4. Compare K-Means clustering with DBSCAN.
5. Profile clusters and discuss potential actions for different customer segments.

## Requirements
Python 3.9 or compatible, pandas, NumPy, scikit-learn, psycopg2-binary, and Jupyter Notebook.

Install the Python dependencies:
```bash
pip install pandas numpy scikit-learn psycopg2-binary jupyter
```

## Running the notebook
The notebook expects the required source data to be available in a local `data/` directory as described in the notebook, or access to the configured PostgreSQL database. Do not commit private datasets, database credentials, or customer-level personal information.

For a database connection, set `PG_LOGIN` and `PG_PASSWORD` as environment variables in your local environment before running the notebook. Keep credentials out of source control.

## Notes
The presentation reports the results of the analysis. Reproduce the results only with authorized data and access. Confirm that the project data and any results shared publicly are permitted by the Academy or data owner.
