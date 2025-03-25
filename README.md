# Digital-Assignment-2
# Linear Regression: AI Technique Report

## *1\. Understanding Linear Regression*

Linear Regression is one of the simplest and most widely used machine learning algorithms for predictive modeling. It establishes a relationship between an independent variable (X) and a dependent variable (Y) using a linear equation:

Where:

* *Y* is the predicted output.  
* *m* is the slope of the line (coefficient for X).  
* *X* is the input feature.  
* *b* is the intercept.

Linear regression is commonly used for forecasting, trend analysis, and predictive modeling in various domains such as finance, healthcare, and business analytics.

### *Mathematical Approach*

Linear regression aims to minimize the error between actual values and predicted values by optimizing the parameters (m and b). This is achieved using:

1. *Ordinary Least Squares (OLS)*: Minimizes the sum of squared residuals.  
2. *Gradient Descent*: Iteratively updates weights to minimize the cost function:  
   Here, J(m, b) represents the mean squared error (MSE).

## *2\. Coding Linear Regression (GitHub Link: \[Your Repo Link Here\])*

### *Dataset Selection*

For this project, we use the *Diabetes Dataset* from sklearn.datasets to predict diabetes progression based on various features such as *Body Mass Index (BMI), blood pressure, and age*. This dataset contains 442 samples and 10 numerical features collected from diabetes patients.

In our Linear Regression model, we use *BMI as the independent variable* to predict *diabetes progression* as the target variable. This is because BMI has a strong correlation with diabetes progression, making it a suitable choice for simple linear regression.

### *Model Evaluation and Results*

After training the *Linear Regression Model* on the *Diabetes Dataset* with *BMI (Body Mass Index) as the independent variable*, we obtained the following results:

* *Slope (m):* 998.58 → This means that for every *1-unit increase in BMI, the predicted diabetes progression increases by **998.58 units*.

* *Intercept (b):* 152.00 → When BMI is *zero, the predicted diabetes progression starts at **152.00* (though a BMI of zero isn’t realistic).

* *Mean Squared Error (MSE):* 4061.83 → This represents the average squared difference between the actual and predicted values.

* *R² Score:* 0.233 → This means that *23.3% of the variation in diabetes progression* is explained by BMI.

### *Analysis of Results*

* The *R² score of 0.233* suggests that *BMI alone does not fully predict diabetes progression*, indicating that other factors (such as blood pressure, glucose levels, or age) play a significant role.

* The model shows a *positive correlation* between BMI and diabetes progression, which aligns with medical research that *higher BMI is linked to increased diabetes risk*.

* While the model’s performance is limited, it effectively demonstrates *Linear Regression in a real-world medical dataset*.

## *4\. Hardware Implementation Idea*

To implement linear regression on hardware, we can use:

### *1\. Raspberry Pi for Real-Time Predictions*

* Load a trained regression model onto Raspberry Pi.  
* Connect IoT sensors to collect real-world data.  
* Predict values in real-time and display insights on an LCD screen.

### *2\. Arduino with Edge AI*

* Deploy a lightweight model on an Arduino board.  
* Use real-world sensor data to make predictions.  
* Provide automated alerts or actions based on predictions.
