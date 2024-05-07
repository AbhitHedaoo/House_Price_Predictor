# **Bengaluru House Price Predictor**

**Overview** - The "Bengaluru House Price Predictor" project is designed to predict the prices of houses in Bengaluru based on various features such as location, size, total square feet area, and number of bathrooms. This project utilizes machine learning techniques, including linear regression, Lasso regression, and Ridge regression, to build predictive models.

**Data Analysis and Cleaning** - The project begins with an analysis of the dataset Bengaluru_House_Data.csv to understand its structure and contents. Data cleaning steps include handling missing values, removing irrelevant columns, and converting data types as needed.
- Removal of columns such as 'area_type', 'availability', 'society', and 'balcony' as they are not relevant for price prediction.
- Handling missing values in columns such as 'location', 'size', and 'bath'.
- Converting the 'total_sqft' column to a standardized format and calculating the price per square foot.
- Grouping locations with fewer occurrences into an 'other' category to reduce dimensionality.
- Detecting and removing outliers in the dataset, specifically focusing on outliers in price per square foot and the number of bedrooms (BHK).
The cleaned dataset is saved as Cleaned_data_House_price_predictor.csv for further analysis and model training.

**Model** - 

**Data Preprocessing**
- One-hot encoding is applied to the categorical feature 'location' using OneHotEncoder.
- Standard scaling is performed to normalize numerical features.

**Model Training**
- The dataset is split into training and testing sets using the train_test_split function.
- Linear regression, Lasso regression, and Ridge regression models are trained using the training data.
- Pipelines are created to streamline the data transformation and model training process.

**Model Evaluation**
- The trained models are evaluated using the R-squared (R2) score, which measures the goodness of fit of the models.
- The performance of each model is assessed by calculating the R2 score on the test data.

**Model Deployment**
- The trained Ridge regression model is saved using pickle as RidgeModel.pkl.
- The saved model can be used for predicting house prices based on new input data.

**Credits** - This project is inspired by tutorials provided by Campus X channel
