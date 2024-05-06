# LAPTOP-PRICE
This project uses machine learning to predict the prices of laptops capturing various features commonly associated with laptops and their corresponding simulated prices.

# PROJECT OVERVIEW
 DATASET
The dataset emulates laptop prices, capturing various features commonly associated with laptops and their corresponding simulated prices. The dataset encompasses the following attributes
1 Company: The manufacturer or brand of the laptop.
2 TypeName: The type or model of the laptop.
3 Inches: The size of the laptop screen, likely measured in inches.
4 ScreenResolution: The resolution of the laptop screen.
5 Cpu: The processor or CPU of the laptop.
6 Ram: The amount of RAM (Random Access Memory) in the laptop.
7 Memory: This likely refers to the storage capacity of the laptop, such as HDD (Hard Disk Drive) or SSD (Solid State Drive).
8 Gpu: The graphics processing unit or GPU of the laptop.
9 OpSys: The operating system installed on the laptop.
10 Weight: The weight of the laptop.
11 Price: The price of the laptop, measured in a floating-point number.

Data Preprocessing: The dataset underwent preprocessing steps such as handling missing values, Remove extra unnecessary details form Product Columns,  Extract CPU Vender, CPU Type and CPU Speed in Different Columns, Convert Ram into Numeric Values, Extract Memory type from Memory Column, Convert Weight into numeric Values, Extract GPU Vender, GPU Type in Different Columns, Extract IPS and Touchscreen Feature form ScreenResolution Column

Model Selection and Pipeline: XGBoost was chosen as the predictive model, integrated into a pipeline with preprocessing steps.

Hyperparameter Tuning: Hyperparameter tuning was conducted using Hyperopt, optimizing the XGBoost model for improved performance.

## RESULT USING XGBOOST
Mean Absolute Error (XGBoost): 9095.43259379921
Mean Squared Error (XGBoost): 205553466.30949795
Root Mean Squared Error (XGBoost): 14337.135917242953
R-squared (XGBoost): 0.8151343726991758

## RESULT USING RANDOM FOREST REGRESSOR
Mean Absolute Error: 9409.167299688701
Mean Squared Error: 249025803.85039103
Root Mean Squared Error: 15780.551443165446
R-squared: 0.7760372896189522

