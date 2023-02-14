# Credit_Risk_Analysis

## **Overview of Credit_Risk_Analysis**

### To study the dataset for PC collected from Amazon and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Use PySpark to determine if there is any bias toward favorable reviews from Vine members in the dataset.

## **Results**

- **How many Vine reviews and non-Vine reviews were there?**

   * The total number of Vine reviews was 1775.
   * The total number of non-Vine reviews was 77370.

  <table>
  <tr>
    <td>The Total Number of Vine and non-Vine Reviews</td>
  </tr>
  <tr>
    <td><img src="Images/Total_Paid_&_Unpaid_Reviews.PNG" width=400></td>
  </tr>
  </table>
  
- **How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?**
  
   * The number of 5-star Vine reviews was 783.
   * The number of 5-star non-Vine reviews was 35944.
  
  <table>
  <tr>
    <td>The Number of 5-star Vine and non-Vine Reviews</td>
  </tr>
  <tr>
    <td><img src="Images/5_star_reviews_Counts.PNG" width=400></td>
  </tr>
  </table>
  
- **What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?**
  
   * The percentage of 5-star Vine reviews was 0.44.
   * The percentage of 5-star non-Vine reviews was 0.46.
   
  <table>
  <tr>
    <td>The Percentages of 5-star Vine and non-Vine Reviews</td>
  </tr>
  <tr>
    <td><img src="Images/5_star_reviews_Percentages.PNG" width=400></td>
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
