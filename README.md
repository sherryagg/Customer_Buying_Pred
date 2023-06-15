# Customer_Buying_Pred

This analysis presents two models that aim to predict whether an e-commerce session will result in a 
purchase and, if so, which of the items clicked in the session will be purchased based on the session’s 
clickstream. The selected models – logistic regression and XGBoost – are applied first on features at 
session level to classify whether a session is going to end with a purchase or not, and then – CatBoost on 
features at item level to predict which items are going to be purchased in that buying session.

The data available consists of two files – the yoochoose-clicks.dat and the yoochoose-buys.dat – covering 
six months going from April to September 2014. In the yoochoose-clicks.dat file, each row corresponds 
to a click on an item that the user has made during a session. The columns are Session ID, Timestamp 
(i.e., when the click occurred), Item ID, Category. In the yoochoose-buys.dat file each row corresponds 
to an item being purchased. The columns are Session ID, Timestamp (when the buy occurred), Item ID, 
Price, Quantity. 
