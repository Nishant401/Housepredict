# HousePredict: House Price Prediction using Linear Regression

This repository contains a machine learning project focused on predicting house prices using linear regression techniques. The project demonstrates the practical application of regression analysis to real estate data.

## Project Overview

HousePredict is a data-driven solution that analyzes various features of residential properties to estimate their market value. By leveraging linear regression, the model identifies key factors that influence house prices and creates a predictive model that can be used for real estate valuation.

## Dataset

The project uses the **House Sales in King County, USA** dataset, which contains house sale prices for King County, Washington between May 2014 and May 2015. The dataset includes homes with various features such as:

- Square footage (living space, lot, basement)
- Number of bedrooms and bathrooms
- Number of floors
- Waterfront presence
- View quality
- Condition and grade of the house
- Year built and renovated
- Zipcode and geographic coordinates (latitude/longitude)

## Features

- **Data Analysis**: Comprehensive exploration and visualization of housing data
- **Feature Engineering**: Creation and selection of relevant features for improved prediction
- **Linear Regression Model**: Implementation of linear regression for price prediction
- **Model Evaluation**: Assessment of model performance using multiple metrics
- **Prediction Interface**: Easy-to-use interface for making new predictions

## Analysis Results

### Correlation Analysis


The correlation matrix reveals important relationships between house features and price:
- Strong positive correlations exist between price and features like square footage, grade, and number of bathrooms
- Living space square footage shows the strongest correlation with price
- Features like year built and zipcode show moderate correlations with price

### Model Performance

The scatter plot of actual versus predicted prices demonstrates the model's predictive capability. The model performs well for houses in the lower to mid-price range, with some deviation for higher-priced properties.

### Residual Analysis

The residual plot reveals:
- Relatively even distribution of residuals around zero for lower-priced homes
- Increasing prediction error (heteroscedasticity) for higher-priced homes
- A sample prediction value of 348,138.03 as shown in the model output

## Technical Implementation

### Data Preprocessing
- Handling of missing values
- Feature scaling and normalization
- Outlier detection and treatment
- Categorical variable encoding

### Model Development
- Feature selection using correlation analysis
- Multiple linear regression implementation
- Regularization techniques (Ridge/Lasso) for preventing overfitting
- Cross-validation for robust model evaluation

### Evaluation Metrics
- R-squared (Coefficient of determination)
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

## Usage

### Prerequisites
- Python 3.6+
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

### How to Use
1. Clone the repository
2. Install the required dependencies
3. Run the Jupyter notebooks to see the data analysis and model building process
4. Use the prediction script to make new house price predictions

## Results

The linear regression model achieved reasonable predictive performance, particularly for houses in the standard price range. The model struggles more with high-end luxury properties, which is consistent with real estate valuation challenges where unique features and limited comparable properties make prediction more difficult.

Key factors influencing price predictions include:
- Square footage of living space
- House grade (quality of construction)
- Number of bathrooms
- Location (zipcode/geographic coordinates)
- Year built

## Future Enhancements

- Integration of additional features such as school district ratings
- Implementation of more advanced regression techniques (Random Forest, Gradient Boosting)
- Development of a web application for interactive predictions
- Address heteroscedasticity with advanced modeling approaches
- Segment analysis for different property types and price ranges

## Contributions

Contributions to this project are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements

- King County Department of Assessments for the housing data
- Kaggle for hosting the dataset
- Various references and resources on regression modeling techniques
