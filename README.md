# Credit Risk Analysis
Project to build machine learning models to assess credit risk using data from Lending Club, peer-to-peer lending services company. Used resampling to attempt to address class imbalance. Evaluated the performance of the machine learning models. Project for UC Berkeley Data Analytics Boot Camp.

### Analysis of Machine Learning Resampling

In order to analyze the data for credit risk and create a prediction model, multiple methods were used involving oversampling, undersampling and ensemble classifier models. The two oversampling models, Naive Random and SMOTE, had nearly the same results. While they had good accuracy rates and great precision for the low-risk data points, they had very poor precision for the high-risk data points.
</br>
I saw similar outcomes with the Cluster Centriods Undersampling and the SMOTEEN combination method. Though their accuracy was not quite as good as the oversampling options, they also had very poor precision rates in predicting the high-risk data points. 
</br>
None of these methods would be very effective in predicting the high-risk credit applications even though they had decent recall rates and found most of the high-risk data points in the samples.
<br>
When using a classifier method, I did see better results for the precision in predicting the high-risk data points. The Easy Ensemble AdaBoost Classifier had the highest accuracy rate (.932) overall as well as the highest precision rate for high-risk data points (.09). The recall rates were also the highest in the testing. Though I saw the best results with the Ensemble Classifier, I would not recommend any of these models for predicting the loan applications. I think it is important to have a high precision rate for high-risk applications to identify those most at risk to the company. I do not think the precision rate for the high-risk applications is strong enough to accurately predict. Since I saw better results with the classifiers, I would recommend further developing the classifier models to try to achieve better precision results without sacrificing the recall and accuracy. 
</br>
Please see outcomes below:
Naive Random Oversampling
Precision High Risk: 0.01, Precision Low Risk: .99
Recall High Risk: 0.70, Recall Low Risk: 0.33
Balanced Accuracy: 0.518

SMOTE Oversampling
Precision High Risk: 0.01, Precision Low Risk: 1.00
Recall High Risk: 0.7, Recall Low Risk: 0.7
Balanced Accuracy: 0.7

Cluster Centroids Undersampling
Precision High Risk: 0.01, Precision Low Risk: 1.00
Recall High Risk: 0.81, Recall Low Risk: 0.47
Balanced Accuracy: 0.643

SMOTEEN
Precision High Risk: 0.01, Precision Low Risk: 1.00
Recall High Risk: 0.71, Recall Low Risk: 0.68
Balanced Accuracy: 0.697

Balanced Random Forest Classifier
Precision High Risk: 0.04, Precision Low Risk: 1.00
Recall High Risk: 0.67, Recall Low Risk: 0.90
Balanced Accuracy: 0.786

Easy Ensemble AdaBoost Classifier
Precision High Risk: 0.09, Precision Low Risk: 1.00
Recall High Risk: 0.92, Recall Low Risk: 0.94
Balanced Accuracy: 0.932


### Tech Used
- Jupyter Notebooks
- Pandas
- Python 3
- NumPy
- scikit-learn
- imblearn

#### Sample of Code
![Code Sample](/image/code.png) 
