# **Spam Prediction Model**

## **Overview**

This project involves building a spam prediction model using **Logistic Regression**. The model was trained to classify whether a given message is spam or not. The key steps include data extraction using **pandas**, text vectorization using **TfidfVectorizer**, and model training with **Scikit-learn**'s Logistic Regression.

## **Project Steps**

1. **Data Extraction**:  
   * The dataset is read using `pandas` for easy manipulation and analysis.  
   * The column containing messages (`df['Message']`) is processed to convert the raw textual data into numerical vectors.  
2. **Text Vectorization**:  
   * The textual data is transformed into numerical vectors using `TfidfVectorizer` from `scikit-learn`.  
   * The parameters used for the vectorizer are:  
     * `min_df=1`  
     * `stop_words='english'`  
     * `lowercase=True`  
3. **Data Splitting**:  
   * After vectorization, the dataset is split into training and testing sets using `train_test_split`.  
   * The split ratio is 80% training data and 20% testing data.  
4. **Model Training**:  
   * A **Logistic Regression** model is trained on the vectorized training data using `scikit-learn`.  
5. **Evaluation**:  
   * The trained model is used to predict spam vs. non-spam on the testing set.  
   * The performance of the model is evaluated using **accuracy score**.

## **Prerequisites**

To run this project, you need the following Python packages installed:

* `pandas`  
* `scikit-learn`  
* `numpy`
