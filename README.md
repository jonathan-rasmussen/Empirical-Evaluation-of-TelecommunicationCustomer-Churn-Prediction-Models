# Empirical Evaluation of Telecommunication Customer Churn Prediction Models

## Project Topic and Selected Option

This project proposal is in accordance with the course requirements of SYDE 675: Pattern Recognition. The topic chosen
 for this project is to conduct an empirical evaluation (Option B) of predicting customer churn rate for telecommunication
 industries. Five machine learning techniques will be implemented and experimented upon to determine the most
 effective technique for prediction. Several datasets were identified for the project, and one or more will be selected for
 training and testing of the techniques. There has been a plethora of academics and industrial research into this business 
problem, several of which are identified in the reference section and have been reviewed. Please see the course website
 for further information.

## Project Description

Customer churn is a phenomenon where businesses lose a percentage of their customer base to competitors. This is
particularly prevalent to telecommunication companies (Telco) whom are consider essential in modern society yet
provide very similar products between competitors. As the Telco industry brings cutting edge technologies such as
fiber optic and 5G networks to the public, it is paramount for them to retain their customers while entering these new 
markets. Extensive research has been conducted in developing customer churn prediction models in the Telco industry.
With accurate detection of customers with a high propensity to attrite, companies can target the customers most likely 
to churn and minimize the limited resources for this endeavour [1]. This proposal seeks to evaluate several state of the 
art machine learning algorithms and their effectiveness to this customer churn problem.

Logistic regression is a statistical method that estimates the parameters of a logistic model. In many applications, it is 
typically considered as a baseline predictive model, and will be treated as such in this proposal [2].

Support vector machines is considered one of the most widely used clustering algorithms in industrial applications
and as such was chosen as one of the potential techniques. The performance of this model will be dependent on the 
separation of the customer classes and effective utilization of kernels [3], [4].

Another technique that will be evaluated is the random forest model. In particular, a unique form of the model known as
 improved balanced random forests will be investigated. This model is a random forest model where the best features are
 iteratively learned by altering the class distribution and by putting higher penalties on misclassification of the minority
 class [5].

 One of the techniques of interest that will be investigated is the XGBoost technique. This technique is an implementation
 of gradient boosted decision trees. Gradient boosting is a technique where new regression tree models are created that
 predict the residuals on prior models [6]. The final prediction of this forest of regression trees can be averaged together 
to correct the errors of the individual trees, providing a more accurate prediction. A key aspect of XGBoost is the
 construction of the forest in parallel, resulting in far faster training times and improved results [7], [8].

 One unique technique utilized in literature is the application of neural networks in churn data. This project will seek to
 replicate the results of Tsai et al [9], whom implemented two hybrid neural networks to customer churn predictions.
 The first hybrid neural network is a combination of two back-propagated artificial neural networks (ANN). The second
 system is a combination of a self-organizing map and an ANN. The propose of this hybrid network is for the first
  network to conduct data reduction, and the second network to predict the customer churn.

## Data Description

The data chosen for the empirical evaluation is the Telco Customer Churn dataset retrieved from Kaggle. The dataset
 was developed by IBM as a sample dataset for a fictional telecommunication company that provided Internet and home
 phone services to customers in California in Q3. The dataset consists of 7043 rows of data where each row represents
 one customer and each column contains information about the customers attributes. The column "Churn" is the target
 column of the dataset which is a binary classification of yes/no indicating if the customer has left the service within the
 last month. The dataset contains 20 feature columns for each customer where the features describe the services that the
 customer has signed up for, the customers account information, and demographic information about the customer.
 Link to data: https://www.kaggle.com/blastchar/telco-customer-churn

A secondary Telco Customer Churn dataset developed by the Teradata center for customer relationship management at
 Duke University was retrieved and included as a backup dataset. This dataset was retrieved from Kaggle and consists of
71,047 unique rows of data and 58 features representing the attributes of one customer between July 2001 to January
 2002. The IBM sample Telco dataset was chosen over the Duke Telco dataset due to the recency of the data. Since the
 Duke dataset was collected in 2002, it contains attributes of a customer that may no longer be relevant today such as
 "handset model" and is missing attributes that are relevant to the current environment such as "wireless Internet".
 Link to secondary data: https://www.kaggle.com/jpacse/datasets-for-churn-telecom

## References

[1] S. A. Qureshi, A. S. Rehman, A. M. Qamar, A. Kamal, and A. Rehman, “Telecommunication subscribers’ churn prediction
model using machine learning,” in8th International Conference on Digital Information Management, ICDIM 2013, 2013,
pp. 131–136,ISBN: 9781479906130.DOI: 10.1109/ICDIM.2013.6693977.

[2] B. Huang, M. T. Kechadi, and B. Buckley, “Customer churn prediction in telecommunications,”Expert Systems with Appli-
cations, vol. 39, no. 1, pp. 1414–1425, Jan. 2012,ISSN: 09574174.DOI: 10.1016/j.eswa.2011.08.024. [Online]. Available:
https://www.sciencedirect.com/science/article/abs/pii/S0957417411011353.

[3] G. E. Xia and W. D. Jin, “Model of customer churn prediction on support vector machine,”Xitong Gongcheng Lilun yu
Shijian/System Engineering Theory and Practice, vol. 28, no. 1, pp. 71–77, Jan. 2008,ISSN: 10006788.DOI: 10.1016/s1874-
8651(09)60003-x. [Online]. Available: https://www.sciencedirect.com/science/article/abs/pii/S187486510960003X.

[4] Y. Zhao, B. Li, X. Li, W. Liu, and S. Ren, “Customer Churn Prediction using improved one-class Support Vector Machine,”
inLecture Notes in Computer Science (including subseries Lecture Notes in Artificial Intelligence and Lecture Notes in
Bioinformatics), vol. 3584 LNAI, Springer Verlag, 2005, pp. 300–306,ISBN: 354027894X.DOI: 10.1007/11527503_36.
[Online]. Available: https://link.springer.com/chapter/10.1007/11527503_36.

 [5] Y. Xie, X. Li, E. W. Ngai, and W. Ying, “Customer churn prediction using improved balanced random forests,”Expert Systems
with Applications, vol. 36, no. 3 PART 1, pp. 5445–5449, Apr. 2009,ISSN: 09574174.DOI: 10.1016/j.eswa.2008.06.121.
[Online]. Available: https://www.sciencedirect.com/science/article/abs/pii/S0957417408004326.

[6] T. Vafeiadis, K. I. Diamantaras, G. Sarigiannidis, and K. C. Chatzisavvas, “A comparison of machine learning techniques for
customer churn prediction,”Simulation Modelling Practice and Theory, vol. 55, pp. 1–9, Jun. 2015,ISSN: 1569190X.DOI: 10.
1016/j.simpat.2015.03.003. [Online]. Available: https://www.sciencedirect.com/science/article/abs/pii/S1569190X15000386.

[7] A. K. Ahmad, A. Jafar, and K. Aljoumaa, “Customer churn prediction in telecom using machine learning in big data platform,”
Journal of Big Data, vol. 6, no. 1, pp. 1–24, Dec. 2019,ISSN: 21961115.DOI: 10.1186/s40537-019-0191-6. [Online]. Available:
https://link.springer.com/article/10.1186/s40537-019-0191-6.

[8] J. Pamina, J. Beschi Raja, S. Sathya Bama, S. Soundarya, M. S. Sruthi, S. Kiruthika, V. J. Aiswaryadevi, and G. Priyanka,
“An effective classifier for predicting churn in telecommunication,”Journal of Advanced Research in Dynamical and Control
Systems, vol. 11, no. 1 Special Issue, pp. 221–229, Jun. 2019,ISSN: 1943023X. [Online]. Available: https://papers.ssrn.com/
abstract=3399937.

[9] C. F. Tsai and Y. H. Lu, “Customer churn prediction by hybrid neural networks,”Expert Systems with Applications, vol. 36,
no. 10, pp. 12 547–12 553, Dec. 2009,ISSN: 09574174.DOI: 10. 1016 / j. eswa. 2009. 05. 032. [Online]. Available: https :
//www.sciencedirect.com/science/article/abs/pii/S0957417409004758.
