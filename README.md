# Spam Email Detection Using Machine Learning

## Overview
This project is a machine learning-based application designed to detect spam emails. It combines data preprocessing, feature extraction, and a logistic regression model to classify emails as either **spam** or **not spam**. Additionally, it integrates the Gmail API to analyze real-world emails and predict their classification.

## Features
- **Data Preprocessing**:
  - Handles missing values.
  - Encodes spam as `0` and non-spam (ham) as `1`.

- **Machine Learning Model**:
  - Logistic Regression is used for spam classification.
  - Achieves a high level of accuracy on training and test datasets.

- **Gmail API Integration**:
  - Authenticates using the Gmail API.
  - Retrieves email content (subject and body) for analysis.
  - Predicts if the retrieved email is spam.

- **Real-time Predictions**:
  - Allows users to input an email text and predict its classification.

---

## Dataset
The model is trained on a labeled dataset (`mail_data.csv`) where:
- `Category` represents whether an email is spam or not.
- `Message` contains the email content.

---

## Technology Stack
- **Programming Language**: Python
- **Libraries Used**:
  - `numpy`, `pandas`: Data manipulation and preprocessing.
  - `scikit-learn`: Machine learning and feature extraction.
  - `googleapiclient`, `google-auth-oauthlib`: Gmail API integration.
  - `BeautifulSoup`: HTML parsing for cleaning email content.

---

## Installation and Usage

### Prerequisites
- Python 3.7+
- Required libraries:
  ```bash
  pip install numpy pandas scikit-learn google-api-python-client google-auth-oauthlib beautifulsoup4
