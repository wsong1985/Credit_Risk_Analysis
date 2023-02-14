# Credit_Risk_Analysis

## **Overview of Credit_Risk_Analysis**

To assist LendingClub in analyzing the credit card credit dataset, use imbalanced-learn and scikit-learn libraries to build models using the following resampling algorithms and ensemble classifiers: RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN, BalancedRandomForestClassifier, and EasyEnsembleClassifier. Evaluate the performance of the abovementioned models and determine whether they should be used to predict credit risk. 

## **Results**

- **Resampling with RandomOverSampler algorithm**

   * The balanced accuracy score was 0.6649.
  <br> 
  <table>
  <tr>
    <td>RandomOverSampler Algorithm Balanced Accuracy Score</td>
  </tr>
  <tr>
    <td><img src="Images/Naive Random Oversampling Accuracy Score.PNG" width=500></td>
  </tr>
  </table> 
  
   * The precision scores for high_risk and low_risk were 0.01 and 1.00.
   * The recall scores for high_risk and low_risk were 0.73 and 0.6.
  <br> 
  <table>
  <tr>
    <td>RandomOverSampler Algorithm Precision and Recall Scores</td>
  </tr>
  <tr>
    <td><img src="Images/Naive Random Oversampling Report.PNG" width=500></td>
  </tr>
  </table>
  
- **Resampling with SMOTE algorithm**
  
   * The balanced accuracy score was 0.6623.
  <br> 
  <table>
  <tr>
    <td>SMOTE Algorithm Balanced Accuracy Score</td>
  </tr>
  <tr>
    <td><img src="Images/SMOTE Accuracy Score.PNG" width=500></td>
  </tr>
  </table> 
  
   * The precision scores for high_risk and low_risk were 0.01 and 1.00.
   * The recall scores for high_risk and low_risk were 0.63 and 0.69.
  <br> 
  <table>
  <tr>
    <td>SMOTE Algorithm Precision and Recall Scores</td>
  </tr>
  <tr>
    <td><img src="Images/SMOTE Report.PNG" width=500></td>
  </tr>
  </table>
  
- **Resampling with ClusterCentroids algorithm**
  
   * The balanced accuracy score was 0.5442.
  <br> 
  <table>
  <tr>
    <td>ClusterCentroids Algorithm Balanced Accuracy Score</td>
  </tr>
  <tr>
    <td><img src="Images/Cluster Centroids Accuracy Score.PNG" width=500></td>
  </tr>
  </table> 
  
   * The precision scores for high_risk and low_risk were 0.01 and 1.00.
   * The recall scores for high_risk and low_risk were 0.69 and 0.4.
  <br> 
  <table>
  <tr>
    <td>ClusterCentroids Algorithm Precision and Recall Scores</td>
  </tr>
  <tr>
    <td><img src="Images/Cluster Centroids Report.PNG" width=500></td>
  </tr>
  </table>
  
- **Resampling with SMOTEENN algorithm**
  
   * The balanced accuracy score was 0.6932.
  <br> 
  <table>
  <tr>
    <td>SMOTEENN Algorithm Balanced Accuracy Score</td>
  </tr>
  <tr>
    <td><img src="Images/SMOTEENN Accuracy Score.PNG" width=500></td>
  </tr>
  </table> 
  
   * The precision scores for high_risk and low_risk were 0.01 and 1.00.
   * The recall scores for high_risk and low_risk were 0.81 and 0.57.
  <br> 
  <table>
  <tr>
    <td>SMOTEENN Algorithm Precision and Recall Scores</td>
  </tr>
  <tr>
    <td><img src="Images/SMOTEENN Report.PNG" width=500></td>
  </tr>
  </table>
  
- **Model with BalancedRandomForestClassifier Algorithm**
  
   * The balanced accuracy score was 0.7888.
  <br> 
  <table>
  <tr>
    <td>BalancedRandomForestClassifier Algorithm Balanced Accuracy Score</td>
  </tr>
  <tr>
    <td><img src="Images/Balanced Random Forest Accuracy Score.PNG" width=500></td>
  </tr>
  </table> 
  
   * The precision scores for high_risk and low_risk were 0.03 and 1.00.
   * The recall scores for high_risk and low_risk were 0.70 and 0.87.
  <br> 
  <table>
  <tr>
    <td>BalancedRandomForestClassifier Algorithm Precision and Recall Scores</td>
  </tr>
  <tr>
    <td><img src="Images/Balanced Random Forest Report.PNG" width=500></td>
  </tr>
  </table>

- **Model with EasyEnsembleClassifier Algorithm**
  
   * The balanced accuracy score was 0.9316.
  <br> 
  <table>
  <tr>
    <td>EasyEnsembleClassifier Algorithm Balanced Accuracy Score</td>
  </tr>
  <tr>
    <td><img src="Images/Easy Ensemble AdaBoost Accuracy Score.PNG" width=500></td>
  </tr>
  </table> 
  
   * The precision scores for high_risk and low_risk were 0.09 and 1.00.
   * The recall scores for high_risk and low_risk were 0.92 and 0.94.
  <br> 
  <table>
  <tr>
    <td>EasyEnsembleClassifier Algorithm Precision and Recall Scores</td>
  </tr>
  <tr>
    <td><img src="Images/Easy Ensemble AdaBoost Report.PNG" width=500></td>
  </tr>
  </table>

## **Summary**

- **Findings:**

  * Based on the results, the model with the EasyEnsembleClassifier algorithm had the highest balanced accuracy score of 0.9316, with the run-up of the BalancedRandomForestClassifier algorithm, which scored 0.7888.

  * All six machine learning algorithms had the same precision score for low_risk loans; however, the EasyEnsembleClassifier algorithm had a higher precision score for high_risk loans than the other algorithms.

  * The EasyEnsembleClassifier algorithm had the highest recall scores for high_risk and low_risk loans among the algorithms.

- **Conclusion:**

  * The machine learning model with the EasyEnsembleClassifer algorithm seems to be the best fit for credit risk prediction.
