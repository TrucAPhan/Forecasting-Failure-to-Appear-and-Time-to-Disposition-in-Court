# Forecasting Failure to Appear and Time to Disposition in Court

This is my Capstone group project. Due to privacy concerns, data, codes, and report will not be published.

## Project Introduction:
The U.S. acquires a dynamic legal system that protects the weak and defends justice and equality for people. Before a case is presented in front of a court, a hearing would be scheduled to justify the legitimation of the case, whether the defendant has admissibility of evidence or dismiss the case without further trials. However, for various reasons, many defendants failed to appear for the hearing. This project aims to analyze factors that potentially impact the probability of failure to appear of defendants, along with exploration of the time-to-disposition of hearing cases. Arguments in this paper will be supported by facts, numbers collected by a Washington state county, and analyzed based on classification and predictive methods such as Logistic Regression, Decision Tree, KNN, Support Vector Machine, and Neutral Network. A limitation of this project is the originality of the data set, as it could not fully represent the whole U.S nation, and the predictive results might be varying depending on the geographical locations of the application.

## Machine Learning Procedures Using Python:
- EDA
  - Visualize patterns of defendant failure to appear (DFA) rate and time to disposition (TTD) of different factors, such as gender, age, etc.
  - Variables Selection according to the Correlation Matrix and Holdout Method
- Modeling: 
  1. Forecasting DFA rate: 
  - Logistic Regression
  - Decision Tree
  - SVM/KNN
  - Neural Network
  2. Forecasting TTD: 
  - Linear Regression
  - Decision Tree
- Models comparision: 
  1. Forecasting DFA rate: 
![alt text](https://github.com/TrucAPhan/Forecasting-Failure-to-Appear-and-Time-to-Disposition-in-Court/blob/d9f2cd6be10765aadd673dc4858c30b6a69c96d8/DFA%20results%20.png)
  2. Forecasting TTD:
![alt text](https://github.com/TrucAPhan/Forecasting-Failure-to-Appear-and-Time-to-Disposition-in-Court/blob/d9f2cd6be10765aadd673dc4858c30b6a69c96d8/TTD%20Result.png)
**Note: MAPE = inf in Linear Regression can arise when  the model predicts a 0-day TTD and causes the metric to fail.**

- Recommendation: **Neutral Network** is recommended as a model to predict the probability of the defendant’s failure to appear for a hearing court. While other models are capable of predicting such behavior, yet Neutral Network captures the highest accuracy rate with an adequate sensitivity toward positive predicted cases. On the other hand, for analyzing the Time to Disposition, **Linear Regression** is highly recommended.
- Conclusion: Being able to predict the probability of individuals that likely to fail to appear in a hearing court can be beneficial toward the criminal justice system. Thereby, implementing machine learning techniques upon judicial decisions related to failure to appear should be concerned as an approach to optimize the law system.


