# Reddit Comment Classifier 

## Introduction
This project is focused on building a model creating a convolutional neural network model to classify Reddit comments into three categories: Medical Doctor, Veterinarian, and Other. The reddit.ipynb notebook shows how to build this model using traditional ML method using Logistics regression and SVM while the Reddit-Neural.ipynb shows the model being built with a Convolutional Neural Network (CNN). The main steps include data preprocessing, model training, evaluation, and using the model for predictions on new data.

## Files and Directories

- Reddit-Neural.ipynb: Jupyter notebook containing the entire workflow from data loading and preprocessing to model training, evaluation, and making predictions.

- Labelled_reddit.csv: The derived dataset after preprocessing and labelling the data appropriately. Note that you don't necessarily need it to run the code 

- Reddit_usernames_comments.csv: The original dataset given also this is the only dataset needed to run the code. The data was splitted appropriately into a train and test for evaluation using a train_test_split function in the ratio 60% and 40% respectively. Again this is the only data needed to run the code as it will be splitted into the train and evaluation data while the code is being run using the train_test_split function

- Reddit_comment_classifier_model.h5: This is the saved model that will be used on your own data and the code to use for the prediction on your data has been provided at the end of the Jupyter notebook

## Data Preparation
- Install Dependencies: Ensure you have Jupyter Notebook installed. Install the dependencies in the requirement.txt file

- Run the code

- Making Predictions on New Data using the commented-out code provided at the end of the notebook

- Data Preparation
Data Extraction: The notebook connects to the PostgreSQL database and extracts the Reddit usernames and comments.
Data Cleaning: Basic data cleaning steps are performed to ensure the data is in a suitable format for training the classifier.
Labeling: The data is prepared by using a search function to label the comments for training purposes. The labels are:
A: Medical Doctor
B: Veterinarian
C: Other
The labelled dataset is split into training and evaluation sets using the train_test_split function

- Model Training
The classifier model is trained using a suitable machine learning algorithm. Of all the algorithms used CNN performed best on this task hence why it was chosen for submission

- Evaluation and Results
The model was evaluated to see its accuracy and performance on the test data while also looking at whether the model overfitted or performed well on the dataset. The CNN model generalized well on this task without overfitting or underfitting it also had a good accuracy score. For the traditional model the logistics regression model performed better. Over all the Neural Network is the best approach to use considering the size of the dataset.
