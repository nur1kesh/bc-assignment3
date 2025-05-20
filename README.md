# 💹 AI Crypto Assistant

An intelligent crypto assistant CLI that provides real-time cryptocurrency data, market stats, and news headlines, powered by CoinGecko, Binance, CryptoPanic APIs, and enhanced with Google Gemini AI for insightful summarization.

---

## 🚀 Features

* 🔍 Understands natural language queries about the top 50 cryptocurrencies.
* 📈 Fetches live market data from **CoinGecko** and **Binance**.
* 📰 Retrieves the latest crypto news headlines from CryptoPanic.
* 🧠 Summarizes the data and query using Google Gemini (via Generative AI).
* 💬 Responds in a conversational format with user-friendly information.
* 🛠️ CLI interface for quick interaction (terminal-based).

---

## 📦 Requirements

* Python 3.8+
* .env file with the following:

    GOOGLE_API_KEY=your_google_gemini_api_key
  CRYPTOPANIC_API_KEY=your_cryptopanic_api_key
  

---

## 📥 Installation

1. Clone the repository:

      git clone https://github.com/yourusername/ai-crypto-assistant.git
   cd ai-crypto-assistant
   

2. Install dependencies:

      pip install -r requirements.txt
   

3. Set up environment variables:

   Create a .env file in the root directory:

      GOOGLE_API_KEY=your_google_gemini_api_key
   CRYPTOPANIC_API_KEY=your_cryptopanic_api_key
   

4. Run the assistant:

      python app.py
   

---

## 🧪 Example Queries

What’s the latest news about Ethereum?
Tell me about Bitcoin price and market cap.
What's the current price of Solana?
Should I buy Dogecoin now?

---

## 🧠 How It Works

1. User Input: A natural query like “Tell me about Ethereum price and news”.
2. Parsing: Identifies which of the top 50 coins the query is about.
3. Data Gathering:

   * CoinGecko: Market cap, rank, CoinGecko price.
   * Binance: Live trading price (USDT pair).
   * CryptoPanic: Latest 5 news headlines.
4. AI Summarization: Uses Google Gemini (`gemini-1.5-flash-latest`) to summarize the above into a concise report.
5. Response Output: Prints a helpful AI-generated summary to the terminal.

---

## 📂 Project Structure

├── app.py                 # Main application logic
├── .env                   # Environment variables (not committed)
├── requirements.txt       # Python dependencies
├── README.md              # You are here

---

## 📚 Dependencies

* requests
* python-dotenv
* google-generativeai

Install via:

pip install requests python-dotenv google-generativeai

---

## 🛑 Disclaimers

* This tool does not offer financial advice.
* AI responses are generated for informational and educational purposes only.
* Always do your own research (DYOR) before investing.

---

## 📃 License

MIT License. Feel free to fork, improve, or adapt.

---

## 🙌 Acknowledgments

* CoinGecko API
* Binance API
* CryptoPanic API
* Google Generative AI (Gemini)
