# Dataset Information

This project utilized the **Malicious URLs Dataset** from Kaggle for training and evaluating machine learning models for phishing URL detection.

## Dataset Source

https://www.kaggle.com/datasets/sid321axn/malicious-urls-dataset

## Dataset Overview

The dataset contains approximately **651,191 URLs** categorized into multiple cybersecurity-related classes, including:

- 428,103 Benign URLs
- 96,457 Defacement URLs
- 94,111 Phishing URLs
- 32,520 Malware URLs

The dataset includes two primary columns:

- `url` → The URL address
- `type` → Classification label indicating the type of URL

## Project Usage

The dataset was used for:

- Data preprocessing and cleaning
- Feature encoding and normalization
- Dataset balancing using SMOTEENN
- Machine learning model training
- Model evaluation and performance comparison
- Phishing and malicious URL classification

## Dataset Sources

The dataset was compiled from multiple publicly available cybersecurity sources, including:

- ISCX-URL-2016 Dataset
- PhishTank
- PhishStorm
- Malware Domain Blacklist
- Additional benign URL repositories

## Note

The original dataset file is not included in this repository due to its large size (~45MB). Please download the dataset directly from Kaggle using the link above.
