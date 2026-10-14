# CIC-IDS2017 — Modeling and Evaluation

## Overview
This project builds and evaluates a baseline machine-learning model using the CIC-IDS2017 network traffic dataset to classify benign traffic and attack traffic.

## Objective
Train a predictive model, evaluate its performance using appropriate metrics, and discuss its limitations for network intrusion detection.

## Dataset
- **Dataset:** CIC-IDS2017
- **Subset:** Tuesday Working Hours
- **Input:** 78 numerical network traffic features
- **Target:** Label
- **Classes:** BENIGN, FTP-Patator, SSH-Patator

The original dataset is available from the [Canadian Institute for Cybersecurity](https://www.unb.ca/cic/datasets/ids-2017.html).

## Tools and Technologies
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Google Colab

## Methodology
1. Loaded the cleaned network traffic dataset.
2. Checked data quality and investigated invalid flow durations.
3. Separated numerical features from the target label.
4. Split the data into training and testing sets.
5. Trained a Decision Tree classifier with class weighting.
6. Evaluated predictions using accuracy, balanced accuracy, precision, recall, macro F1-score, and a confusion matrix.

## Evaluation
The notebook contains the model's actual evaluation metrics and confusion matrix. These results should be used to assess performance across all traffic classes, particularly the less frequent attack classes.

## Limitations
- Class imbalance may affect attack detection.
- A Decision Tree is a baseline model and may not capture every traffic pattern.
- Results on this dataset may not generalize to real-world network traffic.
- Evaluation on independent traffic scenarios would provide stronger evidence of generalization.

## Future Work
- Compare the baseline with Random Forest and other classifiers.
- Investigate feature importance.
- Evaluate models on independent traffic scenarios.
- Explore network intrusion detection techniques.
