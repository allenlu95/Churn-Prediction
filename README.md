# Churn-Prediction
Predict user churn for car riding service

In this project, I performed EDA to explore particular features that impact user churn and later performed gridsearch to find which users are most likely to churn with an 81% f1 score.

In the EDA section, I removed any error in recording, and created box plots for the continuous variables and bar plots for the categorical features. I also binned the categorical variable weekday percentage to get a better visualization of its impact. After visulization I used Random Forest to perform feature selection to see if there were any features I failed to explore in detail. Surely enough, avg_distance traveled seems to be important. In the future I will update this project to include analysis in this area.

In the gridsearch section I tested the main classification algorithms, logistic regression, Random forest, adaboost, and boosted trees. I also plotted an ROC curve for each of them, and they all seem rather close except for logisitc regression which has a lower AUC. Our final model was Graident Boosted Trees, which had an .81 f1 score on the test set.
