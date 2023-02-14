# Credit_Risk_Analysis

## **Overview of Credit_Risk_Analysis**

### To assist LendingClub in analyzing the credit card credit dataset, use imbalanced-learn and scikit-learn libraries to build models using the following resampling algorithms and ensemble classifiers: RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN, BalancedRandomForestClassifier, and EasyEnsembleClassifier. Evaluate the performance of the abovementioned models and determine whether they should be used to predict credit risk. 

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
  
- **BalancedRandomForestClassifier Algorithm**
  
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

- **EasyEnsembleClassifier Algorithm**
  
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

- **Is there any positivity bias for reviews in the Vine program?**

  * According to my study, the percentages of Vine and non-Vine 5-star reviews were extremely close. The calculation for non-Vine reviews was conducted with a large sample size, which allowed a more precise approximation for the outcome. Based on the result, there was no positivity bias for 5-star reviews in the Vine program, or the existing bias was so trivial that it could be neglected.

- **Additional analysis is recommended.**
  
  * Taking a step further, we can conduct a similar test for 4-star reviews to see if the result is similar to the result for 5-star reviews.
  * Based on the result, the percentage of Vine 4-star reviews was 0.34, and the non-Vine 4-star reviews was 0.16. There is a possibe bias for 4-star reviews in the Vine program.
  <table>
  <tr>
    <td>The Percentages of 4-star Vine and non-Vine Reviews</td>
  </tr>
  <tr>
    <td><img src="Images/4_star_reviews_Percentages.PNG" width=400></td>
  </tr>
  </table>
