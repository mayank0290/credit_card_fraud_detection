
# OVERVIEW 📜

**Dataset Description**: 

* The dataset contains transactions spanning two days.

* The dataset is taken from [kaggle]('https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud')
  
* There are 81 fraud cases out of a total of 17,918 transactions.

* The positive class (frauds) in the dataset constitutes approximately 0.45% of the total transactions.


**Features**:

* The dataset consists of numerical input variables resulting from a PCA transformation.

* Features V1 to V28 are principal components obtained through PCA.

* The original features are confidential and not provided.

* The non-transformed features are ‘Time’ (elapsed seconds since the first transaction) and ‘Amount’ (transaction amount).

**Response Variable**:

* The target variable is ‘Class,’ which takes the value 1 for fraud cases and 0 otherwise.

Keep in mind that the dataset is highly unbalanced, making fraud detection challenging


## CREDIT CARD FRAUD DETECTION USING LOGISTIC REGRESSION 🛡️

**SUMMARY OF STEPS**:
Data Loading and Preprocessing:

Libraries Used:

* **Pandas**: For loading and manipulating the dataset. Pandas allows for easy handling of large datasets and offers various functions to clean and preprocess data.
* **Numpy**: For numerical operations and handling arrays. Numpy is efficient for performing mathematical computations on large datasets.
* **Scikit-learn (sklearn)**:
   - Logistic Regression: For implementing the logistic regression model.
   - Pipeline: To streamline the process of scaling and training the model.
   - StandardScaler: To standardize the dataset before training.
accuracy_score: To evaluate the model's performance.

* **Google Colab**: A cloud-based platform that provides a Python environment to run the analysis. It allows access to powerful computing resources and easy sharing of the work.

 **DATA ANALYSIS AND PREPARATION**:

* Pandas was used to explore and clean the dataset, handle missing values, and prepare the data for analysis.
* Numpy helped in performing numerical operations and creating arrays for the model input.
* StandardScaler from sklearn was used to standardize the features, ensuring they are on a similar scale.

**MODEL SELECTION & TRAINING** :

* Logistic Regression: 
   - Why Logistic Regression:  Logistic Regression is a simple yet powerful algorithm for binary classification problems. It predicts the probability of a transaction being fraudulent (binary outcome: fraudulent or not).
   - Implementation: The logistic regression model was trained on the prepared dataset to learn the patterns of fraudulent transactions.
   - Pipeline: Using make_pipeline from sklearn, a pipeline was created to streamline the scaling and training process.
   - Performance: Achieved an accuracy of 0.9926 on training data and 0.9706 on test data, indicating the model's effectiveness in detecting fraudulent transactions.
* **RESULTS** : The model's high accuracy on both training and test data demonstrates its reliability in identifying fraudulent credit card transactions.

The slight drop in accuracy on test data (compared to training data) is typical and suggests good generalization without overfitting.


## ACKNOWLEDGMENT 🙇🏻‍♂️

The dataset has been collected and analysed during a research collaboration of Worldline and the Machine Learning Group (http://mlg.ulb.ac.be) of ULB (Université Libre de Bruxelles) on big data mining and fraud detection.

More details on current and past projects on related topics are available on https://www.researchgate.net/project/Fraud-detection-5 and the page of the DefeatFraud project
