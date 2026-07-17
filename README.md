# NSE Stock Scanner 📈

A **Python-based NSE stock scanner** that calculates **technical indicators for ~2000 NSE-listed stocks** and automatically **pushes the results to Google Sheets** for easy analysis, filtering, and discovery.

This project is designed for traders, investors, and analysts who want **centralized, always-updated technical data** without juggling multiple tools.



## 🚀 Key Features

* 📊 Scans **~2000 NSE stocks** in one run
* 🧮 Computes **popular technical indicators** using Python
* ☁️ **Auto-syncs results to Google Sheets**
* 🔍 Easy filtering, sorting, and discovery inside Sheets
* ⚡ Fully automated & scriptable
* 🧩 Modular design (add/remove indicators easily)

---

## 📈 Technical Indicators Included

The scanner computes a wide range of indicators, including but not limited to:

* **Trend Indicators**

  * SMA (Simple Moving Average)
  * EMA (Exponential Moving Average)
  * MACD
  * ADX

* **Momentum Indicators**

  * RSI
  * Stochastic Oscillator
  * ROC

* **Volatility Indicators**

  * Bollinger Bands
  * ATR

* **Volume Indicators**

  * Volume SMA / EMA
  * OBV

*(Indicators can be extended easily based on your strategy.)*

---

## 🧠 How It Works

1. Fetches **historical price & volume data** for NSE stocks
2. Processes data using **Python technical analysis libraries**
3. Calculates indicators for each stock
4. Structures results into a clean tabular format
5. Pushes data to **Google Sheets via API**
6. Sheet becomes a **live technical scanner dashboard**

---

## 📊 Google Sheets Integration

Google Sheets acts as the **front-end UI**:

* Filter stocks by indicator values
* Sort by RSI, MACD crossover, trend strength, etc.
* Create watchlists
* Add conditional formatting
* Share with teammates

This makes the scanner **non-technical-user friendly** while keeping Python as the backend engine.

---

## 🛠️ Tech Stack

* **Python**
* Pandas / NumPy
* Technical Analysis libraries (e.g. TA-Lib / pandas-ta)
* Google Sheets API
* Google Service Account authentication

---

## 📂 Project Structure

```
├── data/
│   └── raw_price_data/
├── indicators/
│   ├── trend.py
│   ├── momentum.py
│   └── volatility.py
├── sheets/
│   └── google_sheets_client.py
├── scanner.py
├── config.py
├── requirements.txt
└── README.md
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/nse-stock-scanner.git
cd nse-stock-scanner
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Configure Google Sheets API

* Create a Google Cloud project
* Enable Google Sheets API
* Create a Service Account
* Download credentials JSON
* Share your target Google Sheet with the service account email

Update `config.py` with:

* Sheet ID
* Credentials file path

---

## ▶️ Running the Scanner

```bash
python scanner.py
```

Once completed, the Google Sheet will be updated with **latest indicator values for all NSE stocks**.



## 📌 Use Cases

* Daily technical market scan
* Swing trading setups
* Momentum & breakout discovery
* Portfolio monitoring
* Building custom trading strategies

---

## 🔮 Future Enhancements

* ⏱️ Scheduled runs (cron / Airflow)
* 📉 Signal generation (Buy/Sell/Neutral)
* 📬 Alerts via Email / Telegram
* 🧠 Strategy-based scanners
* 🌐 Web dashboard (optional)

---

## ⚠️ Disclaimer

This project is for **educational and research purposes only**. It does not constitute financial advice. Always do your own research before trading.

---

## ⭐ Contributing

Contributions, ideas, and improvements are welcome! Feel free to open an issue or submit a pull request.

---

## 📄 License

MIT License

---

If you find this project useful, consider giving it a ⭐ on GitHub!!
