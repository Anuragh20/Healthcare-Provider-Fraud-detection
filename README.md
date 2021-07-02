**Background to the Case Study:** 
Healthcare programs, in the United States (U.S.), have experienced tremendous growth in patient populations and commensurate costs and Fraud is a major contributor to these inflating healthcare expenses. 

Many healthcare providers settle huge amounts for patients. But some insured individuals or the provider of health services attempt to make fake claims by giving false claim details such as showing fake bills, submitting same bills repeatedly etc.

**Business Objective**
The primary objective is a binary classification task of each of the provider as either a Fraud or a Non-Fraud.Since the data is related to fraud, the dataset is imbalanced as the number of providers, who commit a fraud is very small proportion when compared to the overall dataset.

**Evaluation Metric**
I will be considering the No Fraud cases a Positive class and the Fraud cases as a Negative class. Considering the problem statement and the class imbalance in the dataset, I intend to explore the following parameters: 
  1.Precision and Recall: Since we are dealing with a fraud identification problem with a class imbalance, metrics such as Accuracy do not precisely evaluate the models. Hence,     I will be going for an evaluation metric such as Precision and Recall. 
  2.AUC score: As it gives an overall view of the classification performance of each of the models
  3.F1 score or Macro F1 score (due to class imbalances): In this case both precision and recall are particularly important as we need to cover as many fraud cases as possible       at the same time we need to able to predict the fraud cases very precisely as False Positives can be very costly.


**Research and Papers being referred to:**

**Paper 1:** https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwjE06e3tP7wAhUID2MBHdL1DH4QFjAAegQICxAD&url=https%3A%2F%2Fwww.aaai.org%2Focs%2Findex.php%2FFLAIRS%2FFLAIRS18%2Fpaper%2Fdownload%2F17617%2F16814&usg=AOvVaw2FyoQRNVI-j_xmGqktZHr_

**Summary of Paper 1: **

The objective of the paper is to come up with a Machine Learning model to detect fraud in the claims for medical providers (only publicly available claims data has been used). Random under sampling, (all fraud labels were retained and non-fraud labels are randomly reduced), was used in order to mitigate the effects of class imbalance. Due to a large size of the dataset the authors have preferred the under-sampling approach to the oversampling approach.
A total of 4 different class distribution datasets have been used where random sampling has been used to select the Majority class observations while keeping the whole of minority class data samples intact. The distribution of the Majority and the minority class for the four distributions has been as follows: 50:50, 65:35, 75:25, 80:20.
Decision trees, support vector machines and logistic regression have been used for the classification task due their popularity and no other concrete reason. Instances labelled Fraud are considered as the positive class whereas the non-fraud instances are considered to be the negative class. AUC, FPR and FNR are the evaluation metrics that were used as AUC is a popular measure of a binary classifier for datasets with severe class imbalance.  

**Paper 2:** Medicare Fraud Detection Using Machine Learning Methods | IEEE Conference Publication | IEEE Xplore
**Summary of Paper 2:**

This paper compares the performance of several machine learning models to detect fraud. The performance of Unsupervised, Supervised and other hybrid machine learning approaches has been evaluated. 
The dataset that has been used in this paper is very similar to Paper 1 and both Over sampling and 80:20 under-sampling methods have been used to deal with Class imbalance. Gradient Boosting Machines, Random Forests and Naïve Bayes have been used under the supervised learning techniques. Mahalanobis, K nearest neighbours and Local Outlier Factor techniques have been used under the unsupervised learning techniques as a part of the anomaly detection activity wherein the outliers are treated as the fraud cases. The specific reasons behind the selection of each of these techniques has not been mentioned in the paper. 
Four performance or evaluation parameters have been used to compare the performance of the models – F1 score, G measure [Sqrt(precision*recall)], Mathew’s Correlated Co-efficient (MCC takes into account all the values in the confusion matrix) and Balanced Accuracy (BACC, takes into account both TPR and TNR).
The paper concludes that a better performance was achieved with 80-20 sampling method with supervised methods when compared to unsupervised and hybrid methods. 



