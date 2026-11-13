💰 Tehran House Price Prediction
A machine learning project that predicts apartment prices in Tehran using Random Forest Regression.

✨ Features
🧹 Data cleaning & outlier removal

🎯 Neighborhood target encoding (mean price per m²)

➕ Engineered feature: total amenities

🌲 Random Forest Regression model

📊 Feature importance & prediction visualizations

🛠️ Technologies Used
Language: Python

Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn

Data: CSV file (1632300362534233.csv)

Interface: Jupyter Notebook

🗂️ Data Format
Stored in 1632300362534233.csv with these columns:

Column	Description
Area	Property area (m²)
Room	Number of rooms
Parking	Parking available (bool)
Warehouse	Warehouse available (bool)
Elevator	Elevator available (bool)
Address	Neighborhood
Price	Price in IRR
Price(USD)	Price in USD
Sample
csv
Area,Room,Parking,Warehouse,Elevator,Address,Price,Price(USD)
63,1,True,True,True,Shahran,1850000000,61666.67
79,2,True,True,True,Pardis,550000000,18333.33
95,2,True,True,True,Shahrake Qods,902500000,30083.33
🚀 Usage
Run the notebook:

bash
jupyter notebook house_price_prediction.ipynb
📁 Place 1632300362534233.csv in the project root

▶️ Run all cells sequentially

📈 Results
Metric	Value
📉 MAE	≈ 1.26 B IRR
🎯 R²	≈ 0.84
Top features: 📐 Area (~0.69), 📍 Address (~0.28).
