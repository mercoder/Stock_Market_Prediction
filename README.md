# Stock_Market_Prediction
### Prediction of Amazon stocks using SVM RBF Kernel and SV Linear Regression

## Introduction
Stocks of a company or cooperation refers to all the shares into which the ownership of the
company is divided. It is a form of monetary investment. Most investors claim stocks to be a
profitable source of income. However, to invest in stocks, one would first need to be aware of
how the stock market behaves. An average investor will have to continuously monitor a lot of
data and can often be swayed in the wrong direction by emotion. For those who do not
understand the market well enough, this will be difficult since buying and selling of stocks must
always be done at the right time to earn maximum profits. The solution to this problem is to
analyze the stock history of a brand/company and predict future stocks based on this data.
The rise of the digital information age and AI has brought forth a new way to predict stocks.
Because of the availability of a massive amount of information on stocks online, there is a need
to automate the prediction of day-to-day fluctuation of stocks for new investors.
A computer program can do so and at the same time reduces human errors and provides
greater security to the investors. Hence, we explore tools and technologies in the fields of data
mining, data prediction and pattern recognition. Smart investors use various methods to predict
the market. These include, Point Data Diagrams, K-line diagram analysis etc. Some implement
mathematical analysis on historical data while others implement sentiment analysis on world
news to provide accurate prediction.
The proposed approach is to make use of Support Vector Machines (SVM) with C type
classification and Radial Basis Function. Support Vector Machines is a very specific type of
learning algorithms characterized by the capacity control of the decision function, the use of the
kernel functions and the scarcity of the solution. The input data that is applied to the model is
from Yahoo Finance. This would be implemented in Python using open-source libraries.
The prediction model will notify investors of the rise of decline in stock prices for the next trading
day and hence, allow them to make calculated decisions. Hence, the model will yield readable
results for new investors to follow.

## Experimental Setup
The experimental results of the analysis and prediction of stock market trends of Amazon are
collected using the following setup. The dataset used in the experiment is obtained from Yahoo
Finance. The dataset used contained stock market data of 5 years (09-21-2015 to 12-12-2020),
i.e. 1318 rows and 7 columns- Date, Open, High, Low, Close, Adj Close and Volume of data.
The dataset is divided into two parts, 80% for testing and 20% for training. The experiment was
coded in Python 3.7 language and libraries such as pandas, numpy, matplotlib and sklearn were
used. The stock prices were forecasted for the last days using Support Vector Linear
Regression Model and Support Vector Machine (SVM) using Radial Basis Function (RBF)
Kernel. Matplotlib is used to create graphs that help compare the forecasted adjusted closing
price of the models to the actual adjusted closing price. The experiment was coded on Google
Colab
