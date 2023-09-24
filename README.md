# Industrial-Copper-Modeling
# Problem Statement:
The copper industry deals with less complex data related to sales and pricing. However, this data may suffer from issues such as skewness and noisy data, which can affect the accuracy of manual predictions. Dealing with these challenges manually can be time-consuming and may not result in optimal pricing decisions. A machine learning regression model can address these issues by utilizing advanced techniques such as data normalization, feature scaling, and outlier detection, and leveraging algorithms that are robust to skewed and noisy data. 
Another area where the copper industry faces challenges is in capturing the leads. A lead classification model is a system for evaluating and classifying leads based on how likely they are to become a customer.
# Libraries Used:
* Pandas, numpy
* seaborn, matplotlib.pyplot
* sklearn.metrics for evaluating the model
* sklearn.preprocessing for encoding and scaling data
* sklearn.model_selection for train_test_split and GridSearchCV
* DecisionTreeRegressor for predicting selling price
* DecisionTreeClassifier for predicting status
* streamlit for UI
* pickle for loading and dumping models

This is a Streamlit web application for predicting the selling price and status of industrial copper based on user inputs. It utilizes machine learning models that have been previously trained and saved as pickle files.
# Working of the Application:
A brief overview of how the application works:

The application provides two tabs: "PREDICT SELLING PRICE" and "PREDICT STATUS."

In the "PREDICT SELLING PRICE" tab, the user can select various input parameters such as "Status," "Item Type," "Country," "Application," and "Product Reference." The user also needs to enter values for "Quantity Tons," "Thickness," "Width," and "Customer ID." Once the user clicks the "PREDICT SELLING PRICE" button, the application will use the input data and the previously trained model to predict the selling price, which will be displayed on the screen.

In the "PREDICT STATUS" tab, the user can enter the same input parameters as in the previous tab but also needs to provide a "Selling Price." Clicking the "PREDICT STATUS" button will use the input data and another previously trained model to predict the status of the industrial copper (whether it is "Won" or "Lost").

Note: The application uses specific pickle files to load the trained models, scalers, and encoders. These pickle files must exist and contain the necessary components for the application to function correctly.
