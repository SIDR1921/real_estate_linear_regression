Real Estate Price Prediction using Linear Regression
📝 Project Overview
This project explores the "Real Estate Price Prediction" dataset from Kaggle to predict the price of a house per unit area. A multiple linear regression model is built to understand the relationship between various property features (like house age, location, and proximity to amenities) and their corresponding prices.

The primary goal is to identify which factors most significantly influence real estate prices in this dataset.

💾 Dataset
The data for this project is sourced from Kaggle: Real Estate Price Prediction Dataset.

The dataset contains the following attributes:

X1 transaction_date: The date of the transaction (e.g., 2013.25)

X2 house_age: The age of the house in years

X3 distance_to_the_nearest_MRT_station: Distance to the nearest metro station in meters

X4_number_of_convenience_stores: The number of convenience stores in the vicinity

X5_latitude: The geographical latitude

X6_longitude: The geographical longitude

Y_house_price_of_unit_area: The target variable to be predicted

🚀 How to Run the Project
To run the analysis on your own machine, follow these steps:

Clone the repository:

git clone https://github.com/SIDR1921/real_estate_linear_regression
cd real_estate_linear_regression

Install the necessary libraries:
Make sure you have Python installed. Then, install the required packages using pip.

pip install pandas scikit-learn matplotlib

Run the analysis:
Execute the Python script or Jupyter Notebook containing the code.

python realestatelr.ipynb

📊 Key Findings
After analyzing the data and building the model, the following key insights were discovered:

Distance to MRT is a Key Driver: The strongest predictor of price is the distance to the nearest MRT station. There is a clear and strong negative correlation: the farther a house is from an MRT station, the lower its price per unit area.

Amenities Matter: The number of nearby convenience stores also shows a significant positive correlation with price. More local amenities lead to higher property values.

Transaction Date is Not a Strong Predictor: The date of the transaction showed no clear trend and had very little impact on the house price within the observed period (2012-2013).

💡 Future Improvements
This project provides a solid foundation, but it can be extended in several ways:

Use Advanced Models: Implement more complex models like Random Forest, Gradient Boosting (XGBoost), or Support Vector Machines (SVM) to potentially improve prediction accuracy.

Feature Engineering: Convert the transaction_date into more useful features like "month" and "year" to capture any seasonal effects.

Model Deployment: Deploy the final model as a simple web application using Flask or Streamlit, where a user can input features and get a price prediction in return.