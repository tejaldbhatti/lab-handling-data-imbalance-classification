![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Lab | Handling Data Imbalance in Classification Models

For this lab and in the next lessons we will use the dataset 'Healthcare For All' building a model to predict who will donate (TargetB) and then - how much they will give (TargetD) (will be used for lab on Friday). You will be using `files_for_lab/categorical.csv, numerical.csv, and target.csv` which can be found at this link.
[link to data](https://github.com/ta-data-remote/lab-random-forests/tree/master/files_for_lab)
You will need to download the data locally.  Remember to add the files to your .gitignore.

### Scenario

You are revisiting the Healthcare for All Case Study. You are provided with this historical data about Donors and how much they donated. Your task is to build a machine learning model that will help the company identify people who are more likely to donate and then try to predict the donation amount.

### Instructions

In this lab, we will take a look at the degree of imbalance in the data and correct it using the techniques we learned in the class.  You should fork and clone this Repo and begin a new Jupyter notebook.

Here are the steps to be followed (building a simple model without balancing the data):


**Everyone is starting with the same cleaned data**

 

**Begin the Modeling here**
- Look critically at the dtypes of numerical and categorical columns and make changes where appropriate.
- Concatenate numerical and categorical back together again for your X dataframe.  Designate the TargetB as y.
  - Split the data into a training set and a test set.
  - Split further into train_num and train_cat.  Also test_num and test_cat.
  - Scale the features either by using MinMax Scaler or a Standard Scaler. (train_num, test_num)
  - Encode the categorical features using One-Hot Encoding or Ordinal Encoding.  (train_cat, test_cat)
      - **fit** only on train data, transform both train and test
      - again re-concatenate train_num and train_cat as X_train as well as test_num and test_cat as X_test
  - Fit a logistic regression (classification) model on the training data.
  - Check the accuracy on the test data.

**Note**: So far we have not balanced the data.

Managing imbalance in the dataset

- Check for the imbalance.
- Use the resampling strategies used in class for upsampling and downsampling to create a balance between the two classes.
- Each time fit the model and see how the accuracy of the model has changed.



