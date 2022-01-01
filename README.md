# machine_learning_trading

The goal of this project is to use/test several different machine learing models to see which one best predicts
future stock prices.  After preprocessing the data (importing, scaling, splitting) we build differnt supervised
learning models.  Classification tables and backtest plots are created to see the performance of each model.


## Technologies (pip list)
This project uses Python 3.7
Pandas 1.2.4
Jupyter lab 3.0.14
pyviz 2.1.0
hvplot 0.7.3
numpy 1.20.1
sklearn 0.24.1 (StandardScaler, linear_model, train_test_split)


#Installation Guide
Make sure to install the following dependencies:
Python 
numpy
sql
scikit-learn


#Imported packages:

Orginal Results with short window = 4, Long_window = 20:
  precision    recall  f1-score   support

        -1.0       0.43      0.04      0.07      1804
         1.0       0.56      0.96      0.71      2288

    accuracy                           0.55      4092
   macro avg       0.49      0.50      0.39      4092
weighted avg       0.50      0.55      0.43      4092

# Results by adjusting the size of the Training data set (and using LogisticRegression):
     precision    recall  f1-score   support

        -1.0       0.44      0.33      0.38      1804
         1.0       0.56      0.66      0.61      2288

    accuracy                           0.52      4092
   macro avg       0.50      0.50      0.49      4092
weighted avg       0.51      0.52      0.51      4092


# Results by adjusting the window of the Training data set:
short window =50
long_window= 200

Results: 
              precision    recall  f1-score   support

        -1.0       0.00      0.00      0.00      1694
         1.0       0.56      1.00      0.72      2161

    accuracy                           0.56      3855
   macro avg       0.28      0.50      0.36      3855
weighted avg       0.31      0.56      0.40      3855


Conclusion from using LR model and changing the windows:
It is easy to see that the model can be improved through changing some of the attributes suich as trading windows and model. 
Eventually, there will be decreasing marginal returns to this model without bringing in more and different 
data.


#Usage
Clone the github repository to run this program in Jupyter Lab 
https://github.com/flyfishjay/algo_trading_with_backtesting_risk


#License
GNU 

#Contributors 
Columbia Fintech Bootcamp
Jason Muenzen www.linkedin.com/in/jason-muenzen-mba-frm