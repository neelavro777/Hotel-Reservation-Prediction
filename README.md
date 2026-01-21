## Tech Stack
- **Language**: Python 3.x
- **ML Framework**: LightGBM, scikit-learn
- **Data Processing**: Pandas, NumPy, imbalanced-learn
- **Experiment Tracking**: MLFlow
- **Web Framework**: Flask
- **Cloud Platform**: Google Cloud Platform (GCS, Cloud Run)
- **Containerization**: Docker
- **CI/CD**: Jenkins
- **Version Control**: Git

## Overview
- **Data Ingestion**: Automated data download from GCP buckets
- **Data Preprocessing**: 
  - Handling imbalanced data using SMOTE
  - Feature selection using Random Forest
  - Label encoding for categorical variables
- **Model Training**: 
  - LightGBM classifier with RandomizedSearchCV
  - Hyperparameter tuning
- **Experiment Tracking**: MLFlow for logging parameters, metrics, and artifacts
- **Web Interface**: Flask-based web application for predictions
- **CI/CD Pipeline**: Automated Jenkins pipeline for build and deployment
- **Cloud Deployment**: Containerized deployment on Google Cloud Run

## Folder Structure 

- ```
Hotel-Reservation-Prediction/
│
├── artifacts/                    # Generated artifacts
│   ├── raw/                      # Raw data
│   ├── processed/                # Processed data
│   └── models/                   # Trained models
│
├── config/                       # Configuration files
│   ├── config.yaml               # Main configuration
│   ├── paths_config.py           # Path configurations
│   └── model_params.py           # Model hyperparameters
│
├── custom_jenkins/                      # Jenkins configuration
│   └── Dockerfile                # Jenkins Docker setup
│
├── notebook/                     # Jupyter notebooks
│   └── notebook.ipynb            # Exploratory data analysis
│
├── pipeline/                     # Pipeline scripts
│   └── training_pipeline.py      # Complete training pipeline
│
├── src/                          # Source code
│   ├── data_ingestion.py         # Data ingestion from GCP
│   ├── data_preprocessing.py     # Data preprocessing pipeline
│   ├── model_training.py         # Model training with MLFlow
│   ├── logger.py                 # Logging configuration
│   └── custom_exception.py       # Custom exception handling
│
├── static/                       # Static files (CSS, JS)
│   └── style.css        
├── templates/                    # Flask HTML templates
│   └── index.html                # Web interface
│
├── utils/                        # Utility functions
│   └── common_functions.py       # Common helper functions
│
├── application.py                # Flask application
├── Dockerfile                    # Application Dockerfile
├── Jenkinsfile                   # Jenkins pipeline definition
├── requirements.txt              # Python dependencies
├── setup.py                      # Package setup
└── README.md                     # This file
```
