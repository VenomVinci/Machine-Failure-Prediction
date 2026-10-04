# Machine Failure Prediction

This project is about predicting whether a machine is likely to fail based on its operating conditions.

I used a machine maintenance dataset containing information such as air temperature, process temperature, rotational speed, torque, tool wear, machine type, and failure status.

## What I Did

I worked through the project step by step, starting with understanding and preparing the dataset.

### 1. Data Understanding

* Loaded and explored the dataset
* Checked the columns and data types
* Checked unique values
* Looked for missing values and duplicate data
* Examined the target variable and failure types

### 2. Data Preprocessing

* Removed unnecessary columns
* Separated the features (`X`) and target (`y`)
* Converted the categorical `Type` column into numerical values using One-Hot Encoding
* Split the data into training and testing sets

### 3. Decision Tree

I first built a Decision Tree classifier to understand how a single tree makes predictions.

I also worked with concepts such as:

* Tree depth
* Splitting
* Measuring purity
* `max_depth`

### 4. Random Forest

After the Decision Tree, I built a Random Forest model.

I learned and applied:

* Multiple decision trees
* Bootstrap sampling
* Sampling with replacement
* Random feature selection
* Voting between trees
* `n_estimators`
* `max_depth`
* Out-of-Bag (OOB) evaluation
* Feature importance

The idea was to use many different trees instead of relying on just one tree.

### 5. XGBoost

I then built an XGBoost classifier and compared it with the Random Forest model.

I worked with the idea of **Gradient Boosting**, where trees are built sequentially and each new tree tries to improve the previous predictions.

### 6. Model Evaluation

I evaluated the models using:

* Accuracy
* Precision
* Recall
* Confusion Matrix

I also compared the performance of the Decision Tree, Random Forest, and XGBoost models.

### 7. Making a New Prediction

Finally, I used the trained XGBoost model to make a prediction for a new machine using values such as:

* Air temperature
* Process temperature
* Rotational speed
* Torque
* Tool wear
* Machine type

The model predicts whether the machine is likely to fail or remain OK.

## Models Used

* Decision Tree
* Random Forest
* XGBoost

## Libraries Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* XGBoost

## Dataset Features

The main features used for prediction were:

* Air temperature
* Process temperature
* Rotational speed
* Torque
* Tool wear
* Machine type

The target was whether the machine experienced a failure.
