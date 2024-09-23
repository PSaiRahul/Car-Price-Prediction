# Car Price Prediction Web Application
This is a Car Price Predictive Analysis Web Application built using Flask as the web framework, and Random Forest Regression for predicting the selling price of a car based on several features like year of purchase, present price, kilometers driven, number of previous owners, fuel type, transmission type, etc.

The model has been trained using machine learning techniques and deployed as a web application to predict car prices using user input.

Table of Contents

	•	Features
	•	Installation
	•	Usage
	•	Technologies Used
	•	Model Information
	•	Contributing

 Features

	•	Predict the selling price of a car based on input parameters.
	•	User-friendly web interface for entering car details.
	•	Provides instant predictions.
	•	Responsive design, accessible on both desktop and mobile devices.

 Installation

   	1.	Clone the Repository:
        git clone https://github.com/yourusername/car-price-prediction.git
        cd car-price-prediction
    2.  Set up a virtual environment (optional but recommended):
        python3 -m venv venv
        source venv/bin/activate    # On Windows use `venv\Scripts\activate`
    3.  Install the required dependencies:
        pip install -r requirements.txt
    4.  Download the pre-trained model (ensure the random_forest_regression_model.pkl is available in the project folder).
    5.	Run the application:
        python app.py
    6.  Access the web application:
        Open a browser and go to http://127.0.0.1:5000/ to use the application.

Usage

	•	Open the web application in your browser.
	•	Enter the details of the car you wish to get a price prediction for:
	•	Year of purchase
	•	Showroom Price (in lakhs)
	•	Kilometers Driven
	•	Number of Previous Owners
	•	Fuel Type (Petrol/Diesel/CNG)
	•	Seller Type (Dealer/Individual)
	•	Transmission Type (Manual/Automatic)
	•	Click the “Calculate the Selling Price” button.
	•	The predicted car selling price will be displayed.

Example Inputs:

	•	Year: 2022
	•	Present Price: 8.50 (in lakhs)
	•	Kilometers Driven: 35000
	•	Number of Owners: 1
	•	Fuel Type: Petrol
	•	Seller Type: Dealer
	•	Transmission: Manual

The application will return a predicted selling price, such as “You Can Sell The Car at ₹5.25 lakhs”.

Technologies Used

	•	Python: Main language used to build the application.
	•	Flask: Lightweight web framework for handling web requests.
	•	Sklearn: Machine learning library for training the Random Forest model.
	•	Bootstrap: Front-end framework for responsive UI.
	•	HTML/CSS: For web page structure and styling.
	•	Pickle: To load the pre-trained model.

 Model Information

This project uses a Random Forest Regression model for car price prediction. The features used in the model are:

	•	Year: Year of purchase (transformed to car age by subtracting from the current year).
	•	Present Price: Current showroom price of the car in lakhs.
	•	Kilometers Driven: Total distance the car has been driven.
	•	Owner: Number of previous owners of the car.
	•	Fuel Type: Petrol, Diesel, or CNG.
	•	Seller Type: Dealer or Individual.
	•	Transmission Type: Manual or Automatic.

The model was trained using historical car sales data from Car Dekho Kaggle dataset to predict the resale value of cars.

Contributing

Feel free to contribute to the project by submitting a pull request or opening an issue.

	1.	Fork the repository.
	2.	Create your feature branch (git checkout -b feature/feature_name).
	3.	Commit your changes (git commit -m 'Add feature').
	4.	Push to the branch (git push origin feature/feature_name).
	5.	Open a pull request.

Developed by Sai Rahul Perumalla
