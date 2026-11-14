# 🏠 Tehran House Price Prediction

A machine learning project that predicts apartment prices in Tehran using Python, Pandas and Scikit-learn.

## ✨ Features

- 🧹 Data cleaning (missing values, invalid areas, zero/negative prices)
- 🏘️ Neighborhood encoding using the average price per square meter
- 🛠️ Feature engineering (`Total_Amenities` = Parking + Warehouse + Elevator)
- 🤖 Price prediction with a Random Forest Regressor
- 📊 Model evaluation (MAE and R²) with visualizations
- 🌟 Feature importance chart

## 🛠️ Technologies Used

- **Language:** Python
- **Libraries:** pandas, numpy, scikit-learn, matplotlib, seaborn
- **Environment:** Jupyter Notebook
- **Dataset:** CSV file (`1632300362534233.csv`)

## 🗂️ Data Format

The dataset contains about 3,450 apartment listings (after cleaning) with these columns:

| Column     | Description                              |
|------------|------------------------------------------|
| Area       | Apartment area in square meters          |
| Room       | Number of rooms                          |
| Parking    | Has parking (True/False)                 |
| Warehouse  | Has warehouse/storage (True/False)       |
| Elevator   | Has elevator (True/False)                |
| Address    | Neighborhood name                        |
| Price      | Price in Toman                           |
| Price(USD) | Price in US dollars                      |

### Sample

```csv
Area,Room,Parking,Warehouse,Elevator,Address,Price,Price(USD)
63,1,True,True,True,Shahran,1850000000.0,61666.67
79,2,True,True,True,Pardis,550000000.0,18333.33
136,3,True,True,True,Saadat Abad,11000000000.0,366666.67
```

## ⚙️ How It Works

1. **Load** the dataset with pandas
2. **Clean** the data: convert `Area` to numeric, drop rows with missing `Address`/`Area`/`Price`, remove outliers (`Area >= 2000`) and invalid prices
3. **Encode** `Address` as the mean price per square meter of each neighborhood
4. **Engineer** the `Total_Amenities` feature
5. **Split** the data into 80% training and 20% testing
6. **Scale** `Area` and `Address` with `StandardScaler`
7. **Train** a `RandomForestRegressor`
8. **Evaluate** with MAE and R², and plot actual vs. predicted prices


## 📈 Results

| Metric | Value |
|--------|-------|
| MAE    | ≈ 1.26 billion Toman (≈ 1,260,879,471) |
| R²     | ≈ 0.84 |

## 🔮 Future Improvements

- Try other models (XGBoost, Gradient Boosting)
- Hyperparameter tuning with GridSearchCV
- Add cross-validation
- Build a simple web app for live price prediction
