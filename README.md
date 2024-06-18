Predicting Advertising Costs Based on Sales Targets

A marketing company is helping clients predict their advertising costs based on sales targets using a simple regression model.

Using the Model in Google Colab:

    Importing the Required Libraries:

import pickle

Loading the Trained Model:

# Load the saved regression model using pickle
with open("/content/sample_data/regression.pkl", 'rb') as file:
    pk_model = pickle.load(file)

    Replace "/content/sample_data/regression.pkl" with the actual path to your saved regression model file in Google Colab.

Making Predictions:

# Predicting advertising costs for specific sales values
predictions = pk_model.predict([[50], [100], [150]])

# Displaying the predictions
print("Predicted advertising costs:")
print(predictions)

    Adjust the input values ([[50], [100], [150]]) based on the sales targets you want to predict for.

    Output:

    After executing the code, you will see the predicted advertising costs for the respective sales targets printed in the console.

    Interpreting the Results:
        The predictions provide estimates of the advertising costs required for achieving sales targets of 50, 100, and 150 units.
        Use these predictions to make informed decisions regarding budget allocation for advertising campaigns based on anticipated sales goals.

This example demonstrates how to leverage a saved regression model to forecast advertising expenditures in Google Colab, enhancing decision-making processes for marketing strategies.

