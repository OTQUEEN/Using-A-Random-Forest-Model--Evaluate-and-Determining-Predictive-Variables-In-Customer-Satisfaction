# Using-A-Random-Forest-Model--Evaluate-and-Determining-Predictive-Variables-In-Customer-Satisfaction
Construct and evaluate a model to determine which features are most important to customer satisfaction.

# Introduction. 
This project uses the same dataset the decision tree model project. For the dataset information, data exploration and data cleaning process, [please refer here for more details](https://github.com/OTQUEEN/Constructing-and-Evaluating-a-Model-to-Predict-Customer-Satisfaction-?tab=readme-ov-file#data-exploration-data-cleaning-and-model-preparation)

As the RandomForestClassifier also requires it all categorical columns to be converted to numeric before the model building. This means that we already have the data fully prepared for the model to be built on.

# importing relevant functions
![image](https://github.com/user-attachments/assets/c08205a7-bde7-41d5-9cc1-9e5570accb2c)

# Model building
![image](https://github.com/user-attachments/assets/1c3910c0-0dd4-4972-bb1e-bec5939706c0)

![image](https://github.com/user-attachments/assets/401673d9-c9e8-4ec1-a0ff-5e04159ca1fd)

* The precision score is: 0.950 for the test set, which means of all positive predictions, 95.0% prediction are true positive.
* The recall score is: 0.942 for the test set, which means of which means of all real positive cases in test set, 94.2% are  predicted positive.
* The accuracy score is: 0.941 for the test set, which means of all cases in test set, 94.1% are predicted true positive or true negative.
* The F1 score is: 0.946 for the test set, which means the test set's harmonic mean is 94.6%.

### Comparing the Tuned Decision Tree model to the Tuned Random Forest Model for the best performing model
  [Click here for the Decision Tree scores](https://github.com/OTQUEEN/Constructing-and-Evaluating-a-Model-to-Predict-Customer-Satisfaction-?tab=readme-ov-file#determine-the-best-decision-tree-models-accuracy-precision-recall-and-f1-score)

![image](https://github.com/user-attachments/assets/2c05dc06-10a2-437d-8996-60164a728447)

Sine the Airline company is interested in knowing the most importance feature in determining customer satisfaction, it very importance to plot the feature of importance graph using the champion model.

![image](https://github.com/user-attachments/assets/2c38dc76-c80b-47fb-98d2-9b270edc8028)

# Conclusion and Recommendation
**In summary:**
* The random forest model predicted satisfaction with more than 94.1% accuracy. The precision is over 95% and the recall is approximately 94.2%.
* The random forest model outperformed the tuned decision tree with the best hyperparameters in most of the four scores. This indicates that the random forest model performs better.
* From the confusion matrix, we can see here the model made a high proportion of true positives and true negatives, where the matrix accurately predicted that the customer would be satisfied or dissatified, respectively than the decision tree model.
* The matrix also had a relatively lower number of false positives and false negatives. Indicating that, there was a less proportion in which the matrix innacurately predicted that the customer would be satisfied or dissatified, respectively.

**Recommendation:**
*  Customer satisfaction is highly tied to `'Inflight entertainment'`, `'Seat comfort'`, and `'Ease of Online booking'`. Improving these experiences should lead to better customer satisfaction. 
*  The success of the model suggests that the airline should invest more effort into model building and model understanding since this model semed to be very good at predicting customer satisfaction. 


**Thank you for reading !!!**

To ready more on the Decision Tree Model, [click here](https://github.com/OTQUEEN/Constructing-and-Evaluating-a-Model-to-Predict-Customer-Satisfaction-?tab=readme-ov-file#determine-the-best-decision-tree-models-accuracy-precision-recall-and-f1-score)
