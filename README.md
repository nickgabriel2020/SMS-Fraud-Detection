# SMS-Fraud-Detection

## Project Overview

This repository contains the final project for DS-502: Predictive Analytics at Capitol Technology University. The project develops and evaluates machine learning and deep learning models for detecting fraudulent SMS-related records.

The project uses a dataset containing approximately 250,000 records. The workflow includes data exploration, preprocessing, feature engineering, baseline machine learning models, neural-network development, model training, and performance evaluation.

## Project Objectives

- Develop a predictive model for SMS fraud detection.
- Compare traditional machine learning approaches with a neural-network model.
- Evaluate model performance using accuracy, precision, recall, F1 score, confusion matrices, and cross-validation.
- Examine the strengths and limitations of applying deep learning to fraud detection.
- Consider ethical and real-world deployment issues.

## Models

The overall project evaluates multiple approaches to SMS fraud detection, including Logistic Regression, Random Forest, and a neural-network model.

The code included in this repository contains the LSTM implementation developed during Milestone C. The LSTM uses 32 units, a dropout rate of 0.20, a 16-neuron dense layer, and a sigmoid output layer for binary classification. The model uses the Adam optimizer and binary cross-entropy loss.

## Dataset and Preprocessing

The dataset contains approximately 250,000 records, including legitimate and fraudulent examples.

Data preparation includes:

- Exploratory data analysis.
- Examination of missing values, duplicates, data types, and class distribution.
- Separation of predictor variables and the target variable.
- One-hot encoding of categorical variables.
- Preparation of 19 final input features.
- Division into 200,000 training records and 50,000 testing records.

The dataset itself is not included in this repository because of file size and data-management considerations.

## Results

The neural-network model achieved extremely strong performance on the evaluated dataset.

Key results include:

- Approximately 99.90% training accuracy during the first epoch.
- 100% validation accuracy during the first epoch.
- Final training loss of approximately 1.375 × 10⁻⁹.
- Final validation loss of approximately 3.392 × 10⁻¹⁰.
- Five-fold cross-validation F1 scores of 1.0000, 1.0000, 0.9995, 1.0000, and 1.0000.
- Average cross-validation F1 score of approximately 0.9999.

The exceptionally high results are interpreted in the final report in the context of dataset characteristics, generalization, evolving fraud techniques, and responsible deployment.

## Software and Dependencies

The project was developed using Python and the following major libraries:

- pandas
- NumPy
- matplotlib
- scikit-learn
- TensorFlow
- Keras

A `requirements.txt` file is included in the repository to document the project dependencies.

## Repository Structure

The repository is organized as follows:

```text
SMS-Fraud-Detection/
│
├── README.md
├── requirements.txt
└── Week5_MilestoneC_LSTM_SMS_Fraud_Gabriel.ipynb
```
## Running the Project
The primary project notebook can be opened and executed using Google Colab or a compatible Jupyter environment.

To run the project:

1. Install the required Python packages listed in `requirements.txt`.
2. Open the project notebook.
3. Update the dataset path if necessary.
4. Run the notebook cells in sequence.
5. Review the generated model metrics and evaluation visualizations.

Because the original dataset is not included in the repository, the dataset must be obtained separately and placed in the appropriate location before running the complete workflow.

## Project Documentation

The methodology, results, discussion, limitations, and ethical considerations are documented in the accompanying final project report submitted for DS-502: Predictive Analytics.
