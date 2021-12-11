# chatbot-healthcare

#Dataset
Training dataset : 113 features , 4920 samples
Testing dataset: 113 features, 41 samples
“prognosis” features is used as label.
Label Encoder is used to encode labels to numbers.

#Training, Testing and Cross Validation
clf1  = DecisionTreeClassifier()
clf = clf1.fit(x_train,y_train)

print(clf.score(testx,testy))

Cross-validation:
scores = cross_val_score(clf, x_test, y_test, cv=3)
Print(scores.mean())

#Results
Training Accuracy: 0.97
Testing Accuracy: 0.94

#Imp Functions (code)
Main()  : Main function that gets executed when program is run
Decision_tree_bot(): Main Logic of the Decision Tree
Binary_search_in_tree(): A subfunction in Decision_tree_bot() and does binary search based on users response to the queries of the bot.
Print_disease_to_user(): This function maps the output of the decision tree to one of the diseases that the user is suffering from.

#FutureIm[plementation
Ensemble Techniques like Random Forest can be used as Decision Trees overfit noisy data. But ensemble methods need huge datasets
