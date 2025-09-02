Databricks Data Quality Exploration with DQX

This project demonstrates the implementation of Databricks Data Quality Framework (DQX) to explore data quality capabilities, using a Netflix dataset as a case study.

Project Overview

The goal of this project is to explore and validate the data quality capabilities of DQX by creating checks for real-world datasets. The workflow includes:

Data Acquisition: Downloaded the Netflix dataset from Kaggle
.

Data Corruption Simulation: Introduced additional inconsistencies to test the robustness of the data quality framework.

Data Quality Checks: Implemented checks to:

Ensure no null values in critical columns.

Validate show_id using regex patterns.

Data Segregation:

Valid records → Written to the Bronze layer.

Invalid records → Written to a Quarantine table for further review.

Project Structure
.
├── notebooks/               # Databricks notebooks
│   └── dqx_data_quality.ipynb
├── data/                    # Sample datasets (if included)
├── README.md                # Project documentation
└── requirements.txt         # Python dependencies

Key Features

Implementation of row-level quality checks with DQX.

Separation of valid and invalid records for ETL workflows.

Demonstration of Bronze layer ingestion and quarantine handling.

Flexible design for testing additional data quality rules.

How to Run

Clone the repository:

git clone <repository_url>


Open the notebook in Databricks.

Ensure the Netflix dataset is available in your workspace.

Run the notebook cells sequentially to:

Load and inspect data.

Apply DQX quality checks.

Write valid and invalid records to respective tables.

References

Databricks DQX Documentation

Netflix Dataset on Kaggle
