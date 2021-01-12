# Stock_Market_Prediction
### Prediction of Amazon stocks using SVM RBF Kernel and SV Linear Regression

## Introduction
Stocks of a company or cooperation refers to all the shares into which the ownership of the company is divided. It is a form of monetary investment. Most investors claim stocks to be a profitable source of income. However, to invest in stocks, one would first need to be aware of how the stock market behaves. An average investor will have to continuously monitor a lot of data and can often be swayed in the wrong direction by emotion. For those who do not understand the market well enough, this will be difficult since buying and selling of stocks must always be done at the right time to earn maximum profits. The solution to this problem is to analyze the stock history of a brand/company and predict future stocks based on this data. 
The rise of the digital information age and AI has brought forth a new way to predict stocks. Because of the availability of a massive amount of information on stocks online, there is a need to automate the prediction of day-to-day fluctuation of stocks for new investors. 
A computer program can do so and at the same time reduces human errors and provides greater security to the investors. Hence, we explore tools and technologies in the fields of data mining, data prediction and pattern recognition. Smart investors use various methods to predict the market. These include, Point Data Diagrams, K-line diagram analysis etc. Some implement mathematical analysis on historical data while others implement sentiment analysis on world news to provide accurate prediction. 
The proposed approach is to make use of Support Vector Machines (SVM) with C type classification and Radial Basis Function. Support Vector Machines is a very specific type of learning algorithms characterized by the capacity control of the decision function, the use of the kernel functions and the scarcity of the solution. The input data that is applied to the model is from Yahoo Finance. This would be implemented in Python using open-source libraries. 
The prediction model will notify investors of the rise of decline in stock prices for the next trading day and hence, allow them to make calculated decisions. Hence, the model will yield readable results for new investors to follow. 

## Methodology
Stock Market Prediction can be considered a prediction problem. The process is depicted as follows. 
 
Firstly, the dataset is retrieved from the source and the system reads the required data [Date, Open, High, Low, Close, Volume, Adjusted]. This data has already undergone Data Preprocessing, reduction and normalization. This involves formatting the data in such a way that it can be read easily by the machine. Data reduction is then done by Principal component analysis- a technique of dimensionality reduction. Based on correlation, groups attributes that contain similar information into a single set of attributes, hence, reducing the number of input attributes to the predictive model. This helps decrease the complexity and noise level in the predictive algorithm. The number of distinct groups in the attributes is identified from the Eigenvalues of correlation matrix of all the attributes.Normalization is the process in which data attributes are scaled to fit within a specified range of -1.0 to 1.0 or 0.0 to 1.0. Normalizing input values in training dataset helps speed up the learning phase. Linear transformation of the original data can be done by Min-Max normalization. Min-Max maps a value v of A to v in the range (new_minA , new_max A ), using the formula: - 
  
; where, maxA and min	A are the maximum and minimum values of an attribute A.	 
For the Training Phase, we use the C-classification Support Vector Machine with RBF Kernel predictive model to calculate the prediction variable. The SVM is a machine learning algorithm that employs optimization techniques to optimize the width of this hyperplane. We input the data from the above set to train SVM (RBF, C = 1e3, gamma = 0.1). We also use the SV Linear Regression Model to predict the stock prices. 
The formula that represents the SVM optimization problem is written as: - 
  
The SV Linear Regression model formula is as follows: 
  
These models predict the stock prices of the test dataset. The actual values in the test dataset are compared with the predicted outputs from the models to evaluate performance of the models. Prediction errors are measured in terms of correlation coefficient between prediction and actual value, mean absolute error etc. 


## Experimental Setup
The experimental results of the analysis and prediction of stock market trends of Amazon are collected using the following setup. The dataset used in the experiment is obtained from Yahoo Finance. The dataset used contained stock market data of 5 years (09-21-2015 to 12-12-2020), i.e. 1318 rows and 7 columns- Date, Open, High, Low, Close, Adj Close and Volume of data. The dataset is divided into two parts, 80% for testing and 20% for training. The experiment was coded in Python 3.7 language and libraries such as pandas, numpy, matplotlib and sklearn were used. The stock prices were forecasted for the last days using Support Vector Linear Regression Model and Support Vector Machine (SVM) using Radial Basis Function (RBF) Kernel. Matplotlib is used to create graphs that help compare the forecasted adjusted closing price of the models to the actual adjusted closing price. The experiment was coded on Google Colab. 

## Experimental Results
Figure 1 represents Amazon Stock Prices over the last 5 years. As per the graph, the stock value of Amazon has grown significantly over the last 5 years at a rapid pace. There is even a remarkable spike in stock prices in recent years. 
 
Figure 2 shows a comparative line graph that compares two sets of data on the Y axis- the adjusted closing prices as predicted by the support vector machine model and the actual adjusted closing prices over the last 30 days of the dataset. The graph helps visualize the accuracy of the SVM model. The SVM model shows a training confidence level of 85%.
  
Figure 3 shows a comparative line graph that compares two sets of data on the Y axis- the adjusted closing prices as predicted by the linear regression model and the actual adjusted closing prices over the last 30 days of the dataset. The graph helps visualize the accuracy of the linear regression model. The model shows a training confidence level of 94% and hence is preferred over the SVM Model. 

## Conclusion
Stock Market Prediction of Amazon was done by implementing SVM RBF Kernel Model and SV 
Linear Regression Model. The SVM Model had a testing accuracy of 84% while the SV Linear Regression Model showed a testing accuracy of 94%. The graphs represent the training accuracy, as we can see, SV Linear Regression provides much more accurate results to predict the stock market performance. 

