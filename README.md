# Air-Passengers-Time-Series-Analysis
A comprehensive Time Series Analysis and Forecasting project using the airline passengers dataset. Includes exploratory data analysis, seasonal decomposition, stationarity validation (ADF Test), and predictive modeling using seasonal statistics to forecast domestic airline passenger traffic

This repository contains a step-by-step implementation of **Time Series Analysis and Forecasting** using Python. The goal of this project is to analyze historical monthly passenger counts for a domestic airline and forecast future traffic patterns using statistical time series components.

## 📊 Dataset Overview
The project utilizes the classic **Air Passengers dataset** which contains:
* **Timeline:** Monthly intervals spanning multiple years.
* **Feature Variables:** `Month` (Date index) and `#Passengers` (Total count of passengers per month in thousands).
* **Source:** Integrated via safe Google Drive source links directly inside the environment.

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python 3
* **Data Manipulation:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib`, `seaborn`
* **Statistical Modeling:** `statsmodels` (for Seasonal Decomposition)

---

## 🔍 Project Pipeline

### 1. Data Preprocessing & Cleaning
* Checked for missing (null) values and duplicate records to ensure data integrity.
* Converted the `Month` column from a generic object string type to a standard `datetime64` format.
* Set the transformed timeline index to build a structural time-series DataFrame.

### 2. Exploratory Data Analysis (EDA)
* Plotted the target variable over the timeline to visual structural growth.
* Observed a strong **increasing linear trend** along with **cyclic multi-month patterns**.

### 3. Structural Decomposition
Utilized `statsmodels.tsa.seasonal.seasonal_decompose` to break down the timeline array into distinct sub-components:
* **Trend:** Highlights long-term upwards trajectory.
* **Seasonality:** Pinpoints repetitive seasonal shifts over consistent annual intervals.
* **Residuals:** Extracts the remaining random noise/irregular components.

---

## 🚀 Key Insights & Takeaways
* **Clear Upward Trend:** Passenger volume experiences systematic overall growth annually, indicating overall industry expansion over time.
* **Strong Annual Seasonality:** Highly recurrent peaks and valleys are visible during specific months each year, confirming predictive seasonality useful for resource allocation and inventory management.
