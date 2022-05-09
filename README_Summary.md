# Unit 11 - Risky Business

## Summary of Models and Findings
 
![Credit Risk](Images/credit-risk.jpg)

## Background

Mortgages, student and auto loans, and debt consolidation are just a few examples of credit and loans that people seek online. Peer-to-peer lending services such as Loans Canada and Mogo let investors loan people money without using a bank. However, because investors always want to mitigate risk, a client has asked that you help them predict credit risk with machine learning techniques.

In this assignment I will build and evaluate several machine learning models to predict credit risk using data you'd typically see from peer-to-peer lending services. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans). I have employed different techniques for training and evaluating models with imbalanced classes. I used the imbalanced-learn and Scikit-learn libraries to build and evaluate models using the two following techniques:

1. [Resampling](#Final-Questions---Credit-Risk-Resampling-Techniques)
2. [Ensemble Learning](#Final-Questions---Ensemble-Learning)

# Summary 

## Final Questions - Credit Risk Resampling Techniques

1. Which model had the best balanced accuracy score?

    * 0.9516305810328975 - Simple Logistic Regression
    * 0.9956390296683336 - Naive Random Oversampling
    * **0.9956922891485211 - SMOTE Oversampling**
    * 0.994233960487072  - Undersampling
    * 0.9956656594084273 - Combination (Over and Under) Sampling<br><br>
    
    <u>**Conclusion:**</u>  The **SMOTE Oversampling** has the best balanced accuracy scores based on the values above. But also, the Combination (Over and Under) Sampling is very closed to the best.<br><br>


2. Which model had the best recall score?

    * 0.99			   - Simple Logistic Regression
    * 0.9946347503095336 - Naive Random Oversampling
    * 0.9947379281881964 - SMOTE Oversampling
    * **0.9949958728848535 - Undersampling**
    * 0.9946863392488651 - Combination (Over and Under) Sampling<br><br>
    
    <u>**Conclusion:**</u> The **Undersampling model** have the best recall score based on the values above.<br><br>

3. Which model had the best geometric mean score?

    
    * 0.95			     - Simple Logistic Regression
    * 0.9956384531012427 - Naive Random Oversampling
    * **0.9956917685021270 - SMOTE Oversampling**
    * 0.9942336281612222 - Undersampling
    * 0.9956651111585485 - Combination (Over and Under) Sampling<br><br>
    
    <u>**Conclusion:**</u>   The above figures show that the **SMOTE Oversampling** has the best geometric scores even though the Combination (Over and Under) Sampling is very close to the best.

<br><br><br>


## Final Questions - Ensemble Learning

1. Which model had the best balanced accuracy score?

    * Balanced Random Forest Classifier = 0.7871246640962729
    * **Easy Ensemble Classifier = 0.9254565671948463** <br><br>
    
    <u>**Conclusion**</u>  Beased on the calculated figure, it can be concluded that the **Easy Ensemble Classifiee** gave the best accuracy score<br><br>


2. Which model had the best recall score?

    * Balanced Random Forest Classifier = 0.9063644289450741
    * **Easy Ensemble Classifier = 0.9426910781749491** <br><br>
    
    <u>**Conclusion**</u>  Beased on the calculated figure, it can be concluded that the **Easy Ensemble Classifiee** gave the best recall score<br><br>

3. Which model had the best geometric mean score?

     * Balanced Random Forest Classifier = 0.7778528830594635
    * **Easy Ensemble Classifier = 0.9252927802125857** <br><br>
    
    <u>**Conclusion**</u>  Beased on the calculated figure, it can be concluded that the **Easy Ensemble Classifiee** gave the best geometric mean score<br><br>

4. What are the top three features?

      * The top thre features are:-
        - 0.07376667607601396, 'total_rec_prncp'
        - 0.06390324452717588, 'total_rec_int'
        - 0.06073336071656837, 'total_pymnt_inv'