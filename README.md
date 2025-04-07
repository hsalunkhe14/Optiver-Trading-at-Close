# Optiver Trading at the Close: Kaggle Challenge Solution

## 📋 Project Description
This project was developed as part of the **Optiver Trading at the Close Kaggle Challenge**, which focused on predicting stock price movements during the closing auction on the Nasdaq exchange. The closing auction is a critical trading period where large volumes of stocks are traded, and prices are finalized for the day. The objective was to model and predict the weighted price change during this auction using high-frequency trading data.

## 🎯 Objective
The primary goal was to accurately predict the **target variable**, which represents the weighted price change during the closing auction. This was achieved by leveraging statistical analysis, feature engineering, and machine learning techniques to extract meaningful insights from the provided dataset.

---

## 🛠️ Steps Followed

### 1. Data Analysis and Cleaning
- Conducted **Exploratory Data Analysis (EDA)** to understand patterns, distributions, and anomalies in the dataset.
- Handled missing values in features such as `far_price` and `near_price`.
- Normalized numerical features like `bid_price`, `ask_price`, and `matched_size` for consistent scaling.
- Removed outliers and anomalies to ensure data quality.

### 2. Feature Engineering
- Created new features to enhance predictive power:
  - **Price Spread**: Difference between `ask_price` and `bid_price`.
  - **Size Imbalance Ratio**: Ratio of `imbalance_size` to `matched_size`.
  - **Price Momentum**: Percentage change in `reference_price` over time.
- Aggregated features at different time intervals to capture temporal trends.

### 3. Statistical Analysis
- Performed **pairwise correlation analysis** using Pearson correlation to identify relationships between features and the target variable.
- Conducted **autocorrelation analysis** to study stock performance dependencies across different days.
- Measured stock similarities using clustering techniques like **k-means** and visualized them with **t-SNE** plots.
- Investigated market behavior by analyzing the correlation structure of stock closing trajectories.
- Applied formal statistical tests, including **permutation tests**, to assess market behavior patterns.

### 4. Model Building
- Developed predictive models using various machine learning algorithms:
  - Gradient Boosting Machines (GBM)
  - XGBoost
  - LightGBM
  - Neural Networks
- Applied cross-validation techniques to ensure robust model evaluation and prevent overfitting.

---

## ⚙️ Technologies Used
- **Python**: For data preprocessing, feature engineering, and modeling.
- **Pandas & NumPy**: For data manipulation and analysis.
- **Matplotlib & Seaborn**: For data visualization.
- **Scikit-learn**: For machine learning model development and evaluation.
- **XGBoost & LightGBM**: For boosting-based predictive modeling.
- **t-SNE & K-means Clustering**: For dimensionality reduction and clustering analysis.

---

## 📊 Results Overview
The project successfully predicted stock price movements during the closing auction with high accuracy. The models captured complex patterns in high-frequency trading data, providing valuable insights into market dynamics during this critical trading period.

This solution highlights how a combination of statistical analysis, feature engineering, and machine learning can be used effectively in financial markets for predictive tasks.
