# 📊 Time_Series_Model: Gold Price Prediction with ARIMA & SARIMA Models

A robust time series analysis and forecasting project focused on monthly gold price trends using **ARIMA** and **SARIMA** models. It also features an intuitive **Streamlit interface** for visualising trends, evaluating models, and generating forecasts.

---

## 🔍 Highlights of the Project

### 📈 Complete Time Series Analysis Pipeline:

* Gold price data retrieval via **Yahoo Finance**
* Trend exploration through **visual plots**
* **STL decomposition** to separate components (trend, seasonality, residuals)
* **ADF test** to assess stationarity
* **Differencing techniques** for stationarity correction
* Use of **ACF and PACF plots** to estimate model parameters
* Time series modeling via **ARIMA and SARIMA**
* Forecasting gold prices for the next 12–36 months
* **Model evaluation** with AIC/BIC criteria
* **Model serialization** using Pickle

### 🖥️ Streamlit Dashboard Features:

* Choose between ARIMA or SARIMA models for forecasting
* Adjustable forecast period (up to 36 months)
* Graphical forecasts with **confidence intervals**
* Access to raw data and model diagnostics

---

## 📂 Folder Structure

```
gold-price-prediction/
├── app.py                   # Streamlit interface
├── arima_model.pkl          # Pretrained ARIMA model
├── sarima_model.pkl         # Pretrained SARIMA model
├── model_training.ipynb     # Core notebook with analysis & modeling
├── requirements.txt         # Package dependencies
└── README.md                # Documentation
```

---

## 🚀 How to Get Started

### Step 1: Clone the Repository

```bash
git clone https://github.com/vmaradhya2020/Time_Series_Model.git
cd Time_Series_Model
```

### Step 2: Install Required Libraries

```bash
pip install -r requirements.txt
```

### Step 3: Launch the Streamlit App

```bash
streamlit run app.py
```

---

## 📊 Sample Forecast Output

SARIMA forecast visualization with 95% confidence band:

![SARIMA Forecast](https://github.com/vmaradhya2020/Time_Series_Model/blob/main/GoldForecastVisualisation.pdf)

---

## 🧠 Model Comparison

| Model  | Seasonal? | Stationarity | Best For        | Criteria Used |
| ------ | --------- | ------------ | --------------- | ------------- |
| ARIMA  | ❌ No      | Differenced  | Basic Forecasts | AIC / BIC     |
| SARIMA | ✅ Yes     | Differenced  | Seasonal Data   | AIC / BIC     |

### 💡 Model Tuning Hints:

* **Seasonal spikes in ACF** → Consider SARIMA
* **PACF cut-off** after lag *p* → AR(p) component
* **ACF cut-off** after lag *q* → MA(q) component

---

## 🛠️ Tech Stack

* `Python`
* `Pandas`, `Matplotlib`, `Statsmodels`
* `yfinance` for data acquisition
* `Streamlit` for interactive dashboard
* `Pickle` for model saving/loading

---

## 👤 Contributor

Created by **\[Your Name Here]**
📬 Email: \[[vmaradhya@gmail.com](mailto:vmaradhya@gmail.com)]
🌐 GitHub: [github.com/your-username](https://github.com/vmaradhya2020)

---

## 📦 `requirements.txt` Sample

```
streamlit
pandas
matplotlib
statsmodels
yfinance
python-dateutil
```

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

