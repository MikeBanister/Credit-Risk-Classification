## Credit-Risk-Classification

* The model is built on the client's loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks (presumably credit reports), total_deb (total debt).

# Steps
* Data was collected, features were separated and then all were split into training and testing sets
* A Logistic regression was performed using the training data to make risk classification predictions
* Results from Model 1 were used to inform the construction of Model 2, in this case using oversampling to correct for the imbalance.
* Steps above were repeated and results were analyzed using the same metrics and used to make conclusions about the model's efficacy

# Results

* Machine Learning Model 1:
  * Accuracy: Model is accurate overall however this is primarily based on the true positive results which greatly outnumber the true negative.  
  * ~10.6% false negative rate is very high for an unbalanced dataset.
  * F-Score is concerning for loan status 1 (high risk) underscoring the previous point

* Machine Learning Model 2:
  * Model 2's accuracy was notably higher than model 1, though the increase was relatively small in magnitude going from ~95% to 99%
  * As a result of the oversampling the false negative results were greatly reduced in proportion to the true negative though not a tremendous amount in absolute terms.
  * F-Scores for Model 2 were increased across the board providing a better assurance of accuracy.

# Summary
* Model 2 performed best. We were able to identify a defect in the methodology for Model 1 and correct it.
* This conclusion is borne out by the increased accuracy score, lower defect rate and higher F-Scores.
* Because this model is intended to identify a relatively rare phenomenon compared to the data set at large it was vulnerable to overtraining problems.
  This was resolved in the transition from Model 1 to Model 2 
* Based on these conclusions, Model 2 is recommended
