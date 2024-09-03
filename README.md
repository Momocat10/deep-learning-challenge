# Neural Network Model Report

The purpose of this analysis is to train a machine to help Alphabet Soup (a non-profit organization) predict whether applicants would be successful if funded by the organization or not. 

## Data Preprocessing
For processing the data, the main target variable for this model is "IS_SUCCESSFUL", which indicates whether the funding provided to an organization was used effectively. Featured variables are listed below:
The features used to train the model include:
- "APPLICATION_TYPE": Alphabet Soup application type
- "AFFILIATION": The affiliated sector of the industry of the applicant
- "CLASSIFICATION": Government organization classification for the applicant
- "USE_CASE": The use case for which the funding was requested
- "ORGANIZATION": The type of organization applying for funding
- "STATUS": The active status of the applicant
- "INCOME_AMT": The income classification of the applicant
- "SPECIAL_CONSIDERATIONS": Any special considerations noted in the application
- "ASK_AMT": The amount of funding requested by the applicant

Some variables such as "EIN" and "NAME" were removed because they don't contribute much to the prediction process. 

## Compliling, Training, and Evaluating the Model
The number of neurons varied per layer. On the inital layers, there is more neurons and decrease per layer. Having an additional layer in the third attempt was added to see if it could improve accuracy. The common formatting of the layers consisted of an input layer, some hidden layers, and an output layer. The output layer remains utilizing a sigmoid activation function for binary tasks while some hidden layers remained utilizing ReLu. 

## Model Preformance
While the accuracy rate goal was aimed to be at 75%, it was proven to be quite difficult to achieve that. The highest accuracy percentage acheived was the first attempt at 73.04%. Unfortunately the goal was not met. 

## Steps Taken to Increase Performance: 
Various strategies were employed to improve the model's performance, such as:
- Tuning the number of neurons and layers to find an optimal architecture
- Adjusting learning rates and batch sizes to improve convergence during training
- Implementing regularization techniques like dropout to prevent overfitting
- Conducting data normalization to ensure all features contribute equally to the model

## Summary
The deep learning model created for Alphabet Soup helps predict which applicants are likely to be successful if they receive funding. Although the model works well, it didn't seem to meet accuracy rate minimum. To possibly achieve the accuracy goal, using a different type of model like a Random Forest classifier could be considered. It might be easier to understand and potentially perform better. This could be because Random Forest can handle a variety of features and reduce the risk of overfitting, making it a good fit for our data, especially since many of the features are categorical. This could save time instead of binarizing it. 