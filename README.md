# Credit Card Fraud Detection

## Introduction

In today's digital age, the rise of electronic transactions has necessitated robust systems for detecting and preventing credit card fraud. This project addresses this critical issue by leveraging machine learning techniques to identify fraudulent transactions within a dataset of credit card transactions made by European cardholders in September 2013.

## Dataset Overview

The dataset encompasses transactions occurring over a two-day period, comprising 492 fraudulent transactions out of a total of 284,807. The highly imbalanced class distribution, with frauds accounting for only 0.172% of all transactions, presents a challenging scenario for traditional classification methods. The data is anonymized, processed through Principal Component Analysis (PCA), and unfortunately, the original features and background information remain confidential.

The dataset used in this project is publicly available and can be accessed on Kaggle. You can download it [here](https://www.kaggle.com/mlg-ulb/creditcardfraud).

## Features

The dataset primarily includes numerical input variables resulting from PCA transformation, with 'Time' and 'Amount' being exceptions. 'Time' represents the seconds elapsed between each transaction and the first in the dataset, while 'Amount' denotes the transaction amount. The response variable, 'Class,' is binary, taking a value of 1 in the case of fraud and 0 otherwise.

## Challenge and Evaluation

Given the significant class imbalance, traditional accuracy metrics are inadequate. Instead, we recommend evaluating performance using the Area Under the Precision-Recall Curve (AUPRC). This provides a more nuanced understanding of the model's effectiveness in identifying fraudulent transactions within unbalanced datasets.

## Model Performance

In summary, the logistic regression model initially struggled with fraud detection in an imbalanced dataset, showing a recall of 63% and an F1 score of 73%. In contrast, the neural network performed better with a recall of 82% and an F1 score of 78%. Upon balancing the data, a significant enhancement was observed in the logistic regression model, with its recall surging by 33% to an impressive 96%. Meanwhile, the neural network experienced a more moderate increase in recall, reaching 89%. This highlights the efficacy of data balancing in substantially improving the logistic regression model's performance for fraud detection.

## Data Simulator and Resources

An update in March 2021 introduces a simulator for transaction data, offering a practical handbook on Machine Learning for Credit Card Fraud Detection. Practitioners are encouraged to explore this data simulator and methodologies presented in the handbook for enhanced understanding and application.

## Acknowledgements and Citations

The dataset is a result of collaborative research between Worldline and the Machine Learning Group at ULB. Practitioners are urged to cite relevant works, including those by Andrea Dal Pozzolo, Olivier Caelen, Reid A. Johnson, and Gianluca Bontempi, who have contributed to the development and calibration of probability models for unbalanced classification.

## Getting Started

To run the Jupyter Notebook and explore the project, follow the steps below:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/credit-card-fraud-detection.git
   cd credit-card-fraud-detection
