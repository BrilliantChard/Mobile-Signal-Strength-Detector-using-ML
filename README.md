# 📶 Mobile Signal Strength Predictor Using Machine Learning

## 🔍 Project Overview

This project builds a machine learning model to **predict mobile signal strength (in dBm)** using real-world signal metrics like GPS coordinates, speed, and network type. The goal is to help analyze and predict signal strength in various regions, useful for telecom engineering, planning, and optimization.

---

## 📁 Dataset

The dataset contains the following features:

- `Latitude`: GPS latitude coordinate
- `Longitude`: GPS longitude coordinate
- `Altitude`: Elevation at the point of measurement
- `Speed`: Speed of the device during the signal measurement
- `Network Type`: Type of mobile network (e.g., LTE, 3G, GSM)
- `Signal Strength (dBm)`: Target variable – signal strength in decibels

---

## ✅ Project Tasks

### 1. Load and Inspect Dataset
- Read the CSV file using `pandas`
- Check data types, shape, and preview with `.head()`

### 2. Data Analysis and Visualization
- Summary statistics (`.describe()`)
- KDE plots for feature distributions
- Correlation heatmap
- Scatterplots to observe feature-target relationships

### 3. Data Preprocessing
- Drop irrelevant or non-numeric columns
- Handle missing data if any
- Label Encode `Network Type`
- Normalize/Standardize features using `StandardScaler`
- Split dataset into 80% training and 20% test sets

### 4. Model Training
- Train a `RandomForestRegressor` from `scikit-learn`
- Evaluate performance using:
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
  - R² Score

### 5. Visualization
- **Predicted vs Actual** plot
- **Residual distribution** plot
- **Feature importance** bar chart

---

## 📊 Results

Model performance on test set:
- **MAE**: _e.g._ 2.31 dBm
- **MSE**: _e.g._ 7.84 dBm²
- **R² Score**: _e.g._ 0.91 (Excellent Fit)

---

## 🗺️ Future Work (Optional)
- Visualize predictions on a map using `folium` or `geopandas`
- Add real-time data collection and prediction pipeline
- Explore deep learning alternatives (e.g., LSTM for time-dependent signal trends)

---

## 🧰 Tech Stack

- Python 🐍
- Pandas, NumPy
- Scikit-learn
- Seaborn, Matplotlib
- Jupyter Notebook / Google Colab

---

## 📂 How to Run

1. Clone this repo
2. Place your dataset as `signal_metrics.csv` in the working directory
3. Run the notebook or script to:
    - Preprocess data
    - Train model
    - Visualize results

---

## 🙋 Author

**Chard Odhiambo**  
_Telecom & AI Engineer_

---

## 📜 License

This project is open-source under the [MIT License](LICENSE).
