# Simple Stock Forecasting

A lightweight example of stock price forecasting using only historical closing prices. Designed as a quick-start project for demonstrating time series forecasting with machine learning.

This is a simplified version. For more advanced models and market analysis, see my main repo:  
👉 [Quantitative_finance](https://github.com/kyramichel/Quantitative-Finance-XAI)

---

## 🧠 What It Does

- Predicts the **next day's stock closing price**
- Uses only the `Close` column from a stock price CSV
- Employs a **Random Forest Regressor** (scikit-learn)

---

## 🚀 How to Run (Colab)

1. Upload a CSV file containing historical stock data (must include a `Close` column)
2. Run the notebook cells
3. View the predicted next-day closing price

---

## 🔍 Example Code Snippet

```python
data['Target'] = data['Close'].shift(-1)  # Predict next day's Close
X = data[['Close']]
y = data['Target']
model.fit(X_train, y_train)
pred = model.predict([[X.iloc[-1].values[0]]])

## Sample Output
Predicted next close price: 189.54

📎 Related Projects

Time series models, portfolio analysis, backtesting, signal engineering, and more.
