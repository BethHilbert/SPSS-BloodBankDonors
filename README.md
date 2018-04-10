# IBM SPSS Modeler - Blood Bank Donors

Goal
--------------------
To improve the marketing efforts of a blood bank donation center, reducing marketing cost while also improving donor return rate.  


Data
--------------------
Dataset contains 748 real donors from a blood transfusion center in Taiwan. For each donor there are 5 attributes: recency (months since last donation), frequency (total number of donations), monetary (total cc of blood donated), time (months since first donation), and a binary value representing whether the person donated in March 2007. We downloaded the dataset, naming it "transfusion.txt" and included it in this repository.

Dataset is also available from UCI Machine Learning Repository: http://archive.ics.uci.edu/ml/machine-learning-databases/blood-transfusion/


Process
--------------------
We followed Cross-Industry Standard Process for Data Mining (CRISP-DM). Our target was to predict individuals who are most likely to donate based on their past donation behaviors. We used supervised learning since we knew whether they donated in March. 

Most of our time was spent understanding and preparing the data. To handle outliers, we split the attributes into meaningful groups (known as binning). We renamed values so they could be understood by business users (known as reclassifying). And finally, because only 178 of the 700 participants had donated blood during our target month, we sampled in a way that this small percentage of positive results of our target variable would increase to a reasonable sensitivity level (known as stratifying the sample). 

Using this prepared data, we developed 4 classification models: ANN, Bayesian, Decision Tree, and SVM. Each model was developed in a separate stream. All four streams were used for training, and the final test was run on the decision tree stream. 

Links
--------------------
Report: https://github.com/BethHilbert/SPSS-BloodBankDonors/blob/master/Blood%20Bank%20Report.pdf

Models: https://github.com/BethHilbert/SPSS-BloodBankDonors/tree/master/models


