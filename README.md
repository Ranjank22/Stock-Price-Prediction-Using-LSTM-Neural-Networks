---

### 📈 **Stock Price Prediction using LSTM**  

![Stock Prediction](https://upload.wikimedia.org/wikipedia/commons/thumb/9/90/Candlestick_chart_scheme_03-en.svg/800px-Candlestick_chart_scheme_03-en.svg.png)  

## 📌 **Project Overview**  
This project uses **Long Short-Term Memory (LSTM) neural networks** to predict stock closing prices. We analyze **12+ years (2012–2024) of stock data** from Yahoo Finance, compute key financial metrics, and develop an LSTM-based deep learning model for forecasting.  

## 📊 **Dataset**  
- Source: [Yahoo Finance](https://finance.yahoo.com/)  
- Stock: **Adani Enterprises (ADANIENT.NS)**  
- Time Period: **2012-01-01 to 2024-01-01**  
- Features Used: **Close, High, Low, Open, Volume**  

## ⚙️ **Methodology**  
1. **Data Preprocessing**  
   - Fetched stock data using `yfinance`.  
   - Scaled prices using **MinMaxScaler**.  
   - Created **120-day historical sequences** for training.  

2. **LSTM Model Architecture**  
   - **Three LSTM layers** (128, 64, 32 neurons).  
   - **Dropout (0.2) & Batch Normalization** to prevent overfitting.  
   - **ReLU activation** for stable learning.  

3. **Model Training & Evaluation**  
   - Trained on **95% of data**, validated on **5% unseen data**.  
   - RMSE achieved: **~329.4**.  
   - Compared **predicted vs. actual prices post-2023**.  

## 📈 **Results & Insights**  
- **Visualized historical trends** with **50-day & 200-day moving averages**.  
- **Predicted future stock prices** based on past patterns.  
- **Validated model performance** with real post-2023 data.  

## 🚀 **How to Run the Project**  
### **1️⃣ Clone the repository**  
```bash
git clone https://github.com/yourusername/Stock-Price-Prediction-LSTM.git
cd Stock-Price-Prediction-LSTM
```
### **2️⃣ Install dependencies**  
```bash
pip install -r requirements.txt
```
### **3️⃣ Run the model**  
```bash
python stock_prediction.py
```

## 🛠️ **Technologies Used**  
- **Python, Pandas, NumPy**  
- **TensorFlow/Keras (LSTM Model)**  
- **Scikit-learn (Scaling, Evaluation)**  
- **Matplotlib & Seaborn (Data Visualization)**  
- **Yahoo Finance API**  

## 📌 **Future Improvements**  
✅ Fine-tune hyperparameters for lower RMSE.  
✅ Incorporate external factors (news sentiment, market trends).  
✅ Implement **Transformer-based models** for comparison.  

## 🤝 **Contributing**  
Feel free to **fork**, raise issues, or submit pull requests!  

## 🏆 **Author**  
👤 **Ranjan Kumar** | M.Tech Civil Engineering | IIT Kanpur  

---

This README is engaging, informative, and GitHub-friendly! Let me know if you'd like any modifications. 🚀
