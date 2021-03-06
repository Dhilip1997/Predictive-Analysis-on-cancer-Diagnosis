# Predictive-Analysis-on-cancer-Diagnosis

Problem Statement:

Classify the given variation/mutation based on the evidence from the text-based clinical literature.
Purpose of the project:
Inter-pretation of genetic mutation is done manually and classify every single genetic mutation based on evidence from text-based clinical literature. These task are done with manually by clinical pathologist thus it takes more time in classifying them.

In order to avoid this problem we discovered a Machine learning approach based model to classify them.

Data Source: https://www.kaggle.com/c/msk-redefining-cancer-treatment/

Data-overview:
Two dataset:
1. Training_variants(ID,gene,variation)
This contain the information of the genetic mutation
2. Training_text(ID,Text)

Workflow of the project:
1. Load the dataset and done some text-based preprocessing method.

2. Applied Exploratory Data analysis on the train dataset.

3. Features engineering:

I. Gene feature from dataset -categorical variable

a. Applied Response coding

b. Applied One-hot encoding

II. Variation feature from the dataset-categorical variable

a. Applied Response coding

b. Applied One-hot encoding
III. Text literature

a Applied BOW,TFidf

4. Model implementation:
Applied various kind of model
1.Multinomial-Naive-Bayes
2. Logistic-Regression
3. K-nearest neighbor
4. Linear SVM
5. Random forest
Finally done some stacking model operations.

The final Results of loss taken account for every model:

![per1](https://user-images.githubusercontent.com/37034930/86717427-05899d00-bfd7-11ea-867c-97e921666b36.PNG)

conclusion:

From above the results we can conclude that Logistic Regression and Linear SVM performs well when compared to other models.
Thus the Misclassification Points is about 32.93% and 32.63%.
By this i conclude that it saves 67.07% of time when we manualy classify with them.
