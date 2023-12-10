# PRODIGY_DS_03
# Decision Tree Classifier for Banking Dataset

This repository contains a Jupyter notebook implementing a Decision Tree Classifier to predict outcomes in a banking dataset. The dataset, "bank-full.csv," is loaded and analyzed using Python libraries such as pandas, scikit-learn, and matplotlib. The key steps include data exploration, preprocessing, model training, predictions, and evaluation.

## Dataset Overview

The dataset provides information on various features related to banking clients and their responses to marketing campaigns. The features include 'age', 'duration', 'campaign', 'pdays', 'previous', and the target variable 'y.'

## Code Structure

### 1. Loading and Exploring the Dataset

- The dataset is loaded into a Pandas DataFrame using `pd.read_csv`.
- Basic exploratory analysis is performed using `df.head()`, `df.info()`, `df.describe()`, and `df.isnull().sum()`.

### 2. Feature Selection and Preprocessing

- The selected features ('age', 'duration', 'campaign', 'pdays', 'previous') are stored in the variable `x`.
- The categorical variable 'poutcome' is converted to numeric using Label Encoder.

### 3. Splitting the Dataset

- The dataset is split into training and testing sets using `train_test_split`.
- The split ratio is 80% training and 20% testing, with a random seed of 50 for reproducibility.

### 4. Decision Tree Classifier

- A Decision Tree Classifier is instantiated with 'entropy' as the criterion and a maximum depth of 4.
- The model is trained on the training set using `yTree.fit(x_trainset, y_trainset)`.

### 5. Making Predictions

- Predictions are made on the testing set using `yTree.predict(x_testset)`.

### 6. Model Evaluation

- The accuracy of the model is evaluated using `metrics.accuracy_score`.
- The accuracy score is printed to the console.

### 7. Visualization

- The Decision Tree is visualized using `tree.plot_tree` from scikit-learn and displayed using Matplotlib.

## Dependencies

- pandas
- scikit-learn
- matplotlib

## Instructions

1. Ensure you have the required libraries installed (`pip install pandas scikit-learn matplotlib`).
2. Download the dataset 'bank-full.csv' and update the `csv_path` variable with the correct file path.
3. Run the code step by step in a Jupyter notebook or integrate it into your workflow.
