Data Download and Extraction:

1.It downloads a dataset from a specified URL (DATA_SOURCE_MAPPING) using urllib.
-The downloaded file is then extracted using either ZipFile or tarfile module, depending on the file type.
-Data Preprocessing:

2.After downloading and extracting the data, it loads a CSV file fraudTest.csv into a pandas DataFrame.
-It performs initial data preprocessing steps such as checking for missing values and imputing them with appropriate strategies.
-Categorical variables are factorized to convert them into numerical format for modeling.

3.Model Training and Evaluation:
-It splits the dataset into features (X) and the target variable (y).
-Utilizes the train_test_split function from sklearn to split the data into training and testing sets.
-Initializes a DecisionTreeClassifier from sklearn and fits it to the training data.
-The trained model is used to predict the target variable for the test data.
-Model performance is evaluated using metrics such as accuracy score and classification report.

4.Printing Results:
Finally, it prints out the accuracy of the model and the classification report, which provides precision, recall, and F1-score for each class.
