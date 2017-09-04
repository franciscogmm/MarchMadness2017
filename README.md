# MarchMadness2017
Developed predictive models using R and Python to determine the winners of the NCAA March Madness Competition

This project was done using R and Python, and the results were used as a submission to Deloitte’s March Madness Data Crunch Competition. Team members: Luo Yi, Yufei Long, and Yuyang Yue. Data set can't be shared due to limited permission from the organizer

Also, I'm only uploading my code.

### Of the 64 teams that competed, we predicted Gonzaga University to win. Unfortunately, they lost to University of North Carolina in the finals.

## Data Transformation
- The data that was used to train the initial model was from a data set that contained 2002-2016 team performance data, which included statistics, efficiency ratings, etc.,  from different sources. 
- Each row was a game that consisted of two teams and their respective performance data. 
- For the initial training of the models, we were instructed to use 2002-2013 data as the training set and 2014-2016 data as the testing set. 
- After examining the data, we debated on what would be the way to use it. We finally decided on creating new relative variables that would reflect the difference/ratio of team 1 and team 2’s performance. 
- Feature correlation testing was also done during this phase. The results supported the need for relative variables.
- After transformation, feature correlation testing was repeated. This time, results were much more favorable. 
- Principal Component Analysis was also performed on the new features. We hoped to show which features were the most influential, even before running any machine learning models. 
- Imputation was done to deal with missing values. 

## Feature Selection
- For this project, we opted to remove anything (aside from seed and distance from game location) that wasn’t a performance metric. 
- Some of the variables that were discarded were ratings data since we believed that they were too subjective to be reliable indicators.

## Model Testing
We used three models for this project: Decision Tree, Logistic Regression, and Random Forest.
- Decision Tree – Results were less than favorable for this model. Overfitting occurred and we had to drop it.
- Random Forest (R) – We decided to use the Random Forest model for 2 different reasons: the need to bypass overfitting restrictions and its democratic nature.
- Logistic Regression (Python) – From PCA analysis and Random Forest Model, 5 features were selected for this model. 

### Read the analysis at https://dataontherocks.wordpress.com/2017/04/11/predicting-the-winner-of-march-madness-2017-using-r-python-and-machine-learning/
