
# 🏠 Tehran House Price Prediction

A Machine Learning project focused on predicting residential property prices in Tehran, Iran, using Python and supervised learning techniques.

The project explores housing data, applies data preprocessing and feature engineering techniques, and develops predictive models to estimate property prices.

## 🎯 Problem

Estimating house prices can be challenging due to several factors, including location, property size, number of rooms, and other property characteristics.

This project aims to address this problem by analyzing housing data and developing a Machine Learning model capable of predicting property prices based on relevant features.

## ✨ Features

- **Data Exploration (EDA):** Explore and understand the housing dataset.
- **Data Cleaning:** Identify and handle missing or inconsistent values.
- **Data Preprocessing:** Prepare the dataset for Machine Learning.
- **Feature Engineering:** Transform and create useful features to improve model performance.
- **Data Visualization:** Explore relationships between housing features and property prices.
- **Model Training:** Train a Random Forest Regressor to predict house prices.
- **Model Evaluation:** Evaluate prediction performance using regression metrics.
- **Feature Importance:** Analyze which features contribute most to model predictions.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn [if used]
- Scikit-learn
- Jupyter Notebook
- Git
- GitHub

## ⚙️ Installation & Usage

### 1. Clone the Repository

```bash
git clone [YOUR_REPOSITORY_URL]
```

### 2. Navigate to the Project Directory

```bash
cd [PROJECT_DIRECTORY]
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Project

If the project uses Jupyter Notebook:

```bash
jupyter notebook
```

Open the project notebook and execute the cells sequentially.

## 📊 Model Evaluation

The project uses regression evaluation metrics to measure prediction performance.

### Evaluation Metrics

- **MAE (Mean Absolute Error):** Measures the average absolute difference between actual and predicted prices.
- **R² Score:** Measures how well the model explains the variation in house prices.

### Model Results

| Metric | Result |
|---|---|
| Model | Random Forest Regressor |
| R² Score | Approximately 0.84 |
| MAE | Approximately 1.26 billion IRR |

*Note: These values should be updated after the final model evaluation. Make sure the evaluation is performed on a properly separated test dataset without data leakage.*

## 📖 What I Learned

Through developing this project, I gained practical experience in:

- Exploring and analyzing real-world datasets.
- Performing data cleaning and preprocessing.
- Handling missing values and categorical features.
- Applying Feature Engineering techniques.
- Training supervised Machine Learning models.
- Implementing Random Forest Regression.
- Evaluating regression models using MAE and R².
- Visualizing data and interpreting model results.
- Understanding the Machine Learning workflow from raw data to prediction.

## 🚀 Future Improvements

- Comparing multiple regression algorithms.
- Applying cross-validation and hyperparameter tuning.
- Improving feature selection and engineering.
- Preventing data leakage through proper preprocessing pipelines.
- Developing a web application for interactive house price predictions.
- Experimenting with advanced Machine Learning models.

## 👩‍💻 Author

**Pardis Aghamohammadrafi**

---

- Try other models (XGBoost, Gradient Boosting)
- Hyperparameter tuning with GridSearchCV
- Add cross-validation
- Build a simple web app for live price prediction
