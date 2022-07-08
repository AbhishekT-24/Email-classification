## Kaggle Email Classification Challenge <br>

This challenge used email metadata to classify emails into 8 categories:<br>
1. Updates
2. Personal emails
3. Promotions
4. Forums/mails from professional groups
5. Purchases updates
6. Travel emails - advertisements
7. Spam emails
8. Social emails from social networks

<br>
The idea of this challenge is to use a training set with
defined features and predict the category of the test data set.
<br>
The following steps were conducted in the dataset:<br>

1. **Data pre-processing :**<br/>
   1. Date corrections
   2. Timezone correction
   3. Exploring features and how they are distributed for the categories
   4. Based on (3), selecting the correct features
   <br/>
2. **Selecting a model :** The idea here was to run the model to 
train label 1 at first as every algorithm was giving a low
accuracy for the same. So the idea was to first predict label 1 and then predict the rest.
<em>CatBoostClassifier<em>, a classification
model which performs gradient boosting on decision trees,
was used as the results obtained from this model were the best

### Next Steps <br>

The next steps to improve the F1 score of this model will be to:
1. Use dimensionality reduction to decrease the features
2. Use different features for the two different models for prediction
