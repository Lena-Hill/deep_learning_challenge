# Alphabet Soup Charity Success Predictor

## Overview
This project aims to help Alphabet Soup, a non-profit foundation, predict the success of organizations applying for funding. By leveraging machine learning and neural networks, we analyze historical data of funded organizations to forecast which future applicants will be successful if granted support.

## Features
- **Data Preprocessing**: Cleansing and preparation of a comprehensive dataset of more than 34,000 organizations that received funding from Alphabet Soup.
- **Feature Engineering**: Identification and encoding of relevant features that influence the success of funded organizations.
- **Model Training and Evaluation**: Development of a binary classification model using a deep neural network to predict the success of grant applications.

## Dataset
The dataset contains several features about the organizations that have received funding from Alphabet Soup, including:
- `APPLICATION_TYPE`: Alphabet Soup application type
- `AFFILIATION`: Affiliated sector of industry
- `CLASSIFICATION`: Government organization classification
- `USE_CASE`: Use case for funding
- `ORGANIZATION`: Organization type
- `STATUS`: Active status
- `INCOME_AMT`: Income classification
- `SPECIAL_CONSIDERATIONS`: Special considerations for application
- `ASK_AMT`: Funding amount requested
- `IS_SUCCESSFUL`: Indicator of whether the money was used effectively

## Preprocessing Steps
1. Removal of non-beneficial ID columns, such as `EIN` and `NAME`.
2. Determination of the number of unique entries for each column to identify the features.
3. Binning of categorical variables to reduce the complexity of the model.
4. Encoding of categorical variables using one-hot encoding.
5. Splitting of the dataset into training and testing sets.
6. Standardization of feature variables to ensure efficient model training.

## Model Architecture
The neural network model consists of:
- Input layer with a number of neurons equal to the number of features.
- Two hidden layers with `relu` activation to introduce non-linearity.
- Output layer with a single neuron and `sigmoid` activation to predict the binary outcome.

## Evaluation
The model's performance was evaluated using accuracy and loss metrics on a test dataset not seen during the training phase.

## Usage
To run the model training and evaluation, execute the Jupyter notebook provided in the repository. Ensure that the dataset `charity_data.csv` is accessible in the same directory as the notebook.

## Results
The model achieved an accuracy of approximately 72.51% on the test set, indicating a fair ability to predict the success of funding applications based on the provided features.

## Conclusion
This machine learning project provides a foundational approach to predicting the success of charity funding applications. Further improvements might include hyperparameter tuning, additional feature engineering, or experimenting with different model architectures.
