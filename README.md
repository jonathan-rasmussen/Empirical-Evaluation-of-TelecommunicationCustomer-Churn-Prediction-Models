# Empirical Evaluation of Telecommunication Customer Churn Prediction Models

As the Canadian population continues to grow, there is  increased  pressure  on  telecommunication  companies  to  reach more  customers  while  maintaining  their  current  customer  base. As  new  technologies  such  as  5G  are  introduced,  companies  are finding  it  more  challenging  to  retain  their  previous  customers. As the cost of retaining current customers is fifty times less than acquiring new customers, it is imperative that telecommunication companies  seek  accurate  prediction  methods  to  detect  when  a customer  may  churn  from  their  services.  This  paper  conducts an empirical evaluation of five state of the art models and their application  to  customer  churn  prediction  in  the  telecommunication  industry.  The  five  models,  logistic  regression,  random forest,  support  vector  machines,  XGBoost,  and  artificial  neural networks,   are   applied   to   two   different   datasets,   namely   theCell2Cell  and  the  IBM  telecom  datasets.  Specific  classification metrics  and  sampling  methods  were  determined  in  order  to maximize  the  efficacy  of  the  models.  The  models  were  trained and tested on the two datasets with no sampling and with a 1:1undersampling.  The  results  of  this  analysis  show  that  artificial neural networks are most effective for customer churn prediction when there is no sampling, based on the F1 score. When there is sampling  involved,  the  more  effective  choice  is  a  random  forest model. Overall, no model could be chosen as the clear winner for customer churn as it is heavily dependent on the specific dataset, the  sampling  method  chosen,  and  the  metric  of  interest.
