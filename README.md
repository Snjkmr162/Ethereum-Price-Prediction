# Ethereum Price Prediction using Historical Data & Sentiment Analysis

This project develops a predictive model for Ethereum (ETH) prices by combining **historical market data** with **sentiment analysis** from Wikipedia edits.  
The goal is to enhance the precision and reliability of ETH price forecasts by integrating technical and sentiment-driven indicators.

---

## 📂 Project Structure
- `notebooks/Ethereum_Prediction.ipynb` — full analysis, preprocessing, modeling
- `README.md` — project overview and insights (you’re here!)
---

## 🧠 Main Objectives
- Build a baseline predictive model (Random Forest) for Ethereum price movements.  
- Incorporate **Wikipedia edit sentiment** to test its predictive value.  
- Explore correlations between sentiment trends and ETH volatility.  
- Evaluate performance with precision score and feature engineering (moving averages).  

---

## 🔧 Methods & Approach

### 🔹 Data Sources
- **Historical Price Data**: Collected from Yahoo Finance via `yfinance`.  
- **Sentiment Data**: Extracted from Wikipedia edits of Ethereum-related pages.  
- **Preprocessing**: Converted timestamps into Pandas `DatetimeIndex` for time-series alignment.  

### 🔹 Modeling
- **Baseline**: Random Forest Classifier (sklearn).  
- **Feature Engineering**:
  - Moving averages to reduce autocorrelation.  
  - Sentiment scores from Wikipedia edits.  
- **Evaluation**:
  - Precision score for actual vs. predicted values.  

### 🔹 Key Inquiries
- Can Wikipedia edit sentiment offer predictive insights into ETH prices?  
- How does sentiment behave during **major events** (e.g., regulations, Ethereum 2.0 updates)?  
- Are there patterns in sentiment that align with ETH market volatility?  

---

## 📊 Results & Insights
- **Random Forest** gave a solid baseline performance.  
- Sentiment features showed some correlation with ETH volatility, especially around **market-moving events**.  
- More advanced architectures (e.g., Gradient Boosting, LSTMs) could likely improve results.  

---

## 📈 Visualization
- Time-series plots of ETH price and sentiment signals.  
- Moving average smoothing to highlight underlying trends.  
- Comparative charts for predicted vs. actual values.  
---

## 🔍 Analysis & Findings
- Wikipedia edit sentiment provides **non-traditional signals** that sometimes align with market moves.  
- Sentiment fluctuations were strongest around **major announcements** and **regulatory events**.  
- Precision-based evaluation highlighted room for improvement with more complex models.  

---

## 📌 Key Learnings
- Combining sentiment with historical price data is a promising hybrid approach.  
- Random Forest is a good starting point but limited for sequential, time-dependent data.  
- Future work should explore **time-series ML models** (ARIMA, LSTM, Transformers).  

---

## 📚 Requirements
- Python 3.11  
- Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn, yfinance, jupyter.
