# CO₂ Emissions Prediction from Vehicle Data

## Overview

This project builds a machine learning model to predict a vehicle's CO₂ emissions (in g/km) based on its technical specifications. The primary goal is to demonstrate a standard machine learning workflow using a linear regression model and a Scikit-learn Pipeline.

## Dataset

The dataset used is sourced from the Canadian government and contains detailed information on various vehicle models, including their engine specifications, fuel consumption ratings, and corresponding CO₂ emissions.

### Key Features:
- **Engine_Size_L**: The size of the engine in liters.
- **Cylinders**: The number of cylinders.
- **Fuel_Consumption_Comb_L_100km**: Combined fuel consumption (city/highway) in liters per 100 km.
- **CO2_Emissions_g_km**: The target variable for prediction.

## Methodology

The project follows a comprehensive data science methodology:
1. **Data Loading and Cleaning**: Load the dataset and standardize column names for consistency.
2. **Exploratory Data Analysis (EDA)**: Visualize the relationships between features using a seaborn.pairplot to identify correlations.
3. **Model Training**: A linear regression model is trained within a Scikit-learn Pipeline. The pipeline automatically handles feature scaling using StandardScaler before training the model.
4. **Model Evaluation**: The model's performance is evaluated using key regression metrics:
   - Mean Absolute Error (MAE)
   - Mean Squared Error (MSE)
   - R-squared (R2) Score


## Key Findings
- The model achieves a high R-squared (R2) score, indicating a strong linear relationship between the selected features and CO₂ emissions.
- The Fuel_Consumption_Comb_L_100km feature is found to have the most significant positive coefficient, suggesting it is the strongest predictor of CO₂ emissions.
- The use of a Pipeline ensures a clean and reproducible workflow, as it automates both data scaling and model training.

## How to Run the Code

To replicate this analysis, follow these steps:
1. **Clone the repository**:
   ```
   git clone https://github.com/ifedayofakayode/linear-regression.git
   cd linear-regression
   ```
2. **Install dependencies**:
   ```
   pip install pandas numpy scikit-learn seaborn matplotlib
   ```
3. **Download the dataset**: Ensure the CO2 Emissions_Canada.csv file is placed in the data directory as specified in the notebook.
4. Run the Jupyter Notebook:
   ```
   jupyter notebook
   co2-emmission-lr.ipynb
   ```

## Technologies Used

- **Python**
- **Pandas**: For data manipulation and analysis.
- **Scikit-learn**: For model building and evaluation.
- **Seaborn & Matplotlib**: For data visualization.

## 📬 Contact

👤 Ifedayo Fakayode

[LinkedIn](https://www.linkedin.com/in/ifedayofakayode/)
