# customer_churn_logistical_regresion
Do Logistic Regression, then, create a model for a telecommunication company, to predict when its customers will leave for a competitor, so that they can take some action to retain the customers.


What is the difference between Linear and Logistic Regression?
While Linear Regression is suited for estimating continuous values (e.g. estimating house price), it is not the best tool for predicting the class of an observed data point. In order to estimate the class of a data point, we need some sort of guidance on what would be the most probable class for that data point. For this, we use Logistic Regression.

Recall linear regression:

As you know, Linear regression finds a function that relates a continuous dependent variable, y, to some predictors (independent variables  𝑥1
 ,  𝑥2
 , etc.). For example, simple linear regression assumes a function of the form:

𝑦=𝜃0+𝜃1𝑥1+𝜃2𝑥2+⋯
 

and finds the values of parameters  𝜃0,𝜃1,𝜃2
 , etc, where the term  𝜃0
  is the "intercept". It can be generally shown as:

ℎ𝜃(𝑥)=𝜃^𝑇𝑋
 
Logistic Regression is a variation of Linear Regression, used when the observed dependent variable, y, is categorical. It produces a formula that predicts the probability of the class label as a function of the independent variables.

Logistic regression fits a special s-shaped curve by taking the linear regression function and transforming the numeric estimate into a probability with the following function, which is called the sigmoid function 𝜎:

<img width="1013" alt="Screenshot 2024-09-10 at 14 10 51" src="https://github.com/user-attachments/assets/16ecf2c3-68a0-4182-b490-e392ae8b9ea3">

 
In this equation,  𝜃𝑇𝑋
  is the regression result (the sum of the variables weighted by the coefficients), exp is the exponential function and  𝜎(𝜃𝑇𝑋)
  is the sigmoid or logistic function, also called logistic curve. It is a common "S" shape (sigmoid curve).

So, briefly, Logistic Regression passes the input through the logistic/sigmoid but then treats the result as a probability:

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-ML0101EN-SkillsNetwork/labs/Module%203/images/mod_ID_24_final.png" width="400" align="center">
The objective of the Logistic Regression algorithm, is to find the best parameters θ, for  ℎ𝜃(𝑥)
  =  𝜎(𝜃𝑇𝑋)
 , in such a way that the model best predicts the class of each case.
