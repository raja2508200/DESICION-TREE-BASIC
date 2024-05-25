# DESICION-TREE-BASIC

Loading the Data:

The dataset is loaded into a pandas DataFrame from a CSV file named 'desicion tree.csv'.
Preparing the Data:

The feature set X is created by dropping the 'target' column from the DataFrame.
The target variable y is extracted as the 'target' column from the DataFrame.
Splitting the Data:

The dataset is split into training and testing sets using an 80-20 split. This means 80% of the data is used for training the model, and 20% is reserved for testing its performance. The random_state=42 parameter ensures the split is reproducible.
Training the Model:

A Decision Tree Classifier is instantiated with the following parameters:
criterion='entropy': This means the model will use the entropy measure to decide the quality of splits.
random_state=42: This ensures reproducibility of the model.
max_depth=5: This limits the maximum depth of the tree to 5 levels, which helps prevent overfitting.
min_samples_leaf=5: This ensures that each leaf node has at least 5 samples, which also helps prevent overfitting.
The model is then trained using the training data (X_train, y_train).
Making Predictions:

The model is used to make predictions on the test data (X_test).
Evaluating the Model:

The accuracy of the model is calculated using the accuracy_score function from scikit-learn, which compares the predicted labels (y_pred) with the actual labels (y_test).
Predicting on New Data:

The trained model is used to make a prediction on a new data point: [55, 1, 0, 132, 353, 0, 1, 132, 1, 1.2, 1, 1, 3]. This data point represents the features of a new sample, and the model outputs its prediction for the target variable.
Results
Model Accuracy:

The accuracy score of the model on the test data is calculated. This score indicates the percentage of correct predictions made by the model on the unseen test data. Let's assume the calculated accuracy is X%.
New Data Prediction:

For the given new data point [55, 1, 0, 132, 353, 0, 1, 132, 1, 1.2, 1, 1, 3], the model predicts a target value. This predicted value indicates the class to which the new sample is likely to belong.
