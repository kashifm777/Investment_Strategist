# 📈 AI Investment Strategist

This Streamlit application empowers you with AI-driven insights to make informed investment decisions. By leveraging the `agno` library and Google's Gemini models, it analyzes stock performance, researches company fundamentals, and provides potential investment recommendations.

## ✨ Features

* **Stock Performance Analysis:** Retrieves and compares the performance of multiple stocks over the past 6 months using Yahoo Finance data.
* **Company Research:** Fetches detailed company information, including sector, market capitalization, business summary, and the latest news.
* **AI-Powered Insights:** Utilizes specialized AI agents to analyze market trends, company fundamentals, and generate potential investment recommendations.
* **Comprehensive Investment Report:** Aggregates stock performance analysis, company research, and AI-driven recommendations into a structured and investor-friendly report.
* **Interactive Stock Chart:** Visualizes the historical stock prices of the selected companies over the last 6 months using Plotly for better understanding of their trends.
* **User-Friendly Interface:** A clean and intuitive Streamlit interface for easy input of stock symbols.

## 🚀 How to Use

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/kashifm777/Investment_Strategist
    cd ai-investment-strategist
    ```
2.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Set up Google API Key:**
    * Ensure you have a Google Cloud Project with the Generative AI API enabled.
    * Obtain an API key for the Generative AI service.
    * Create a `.env` file in the project root and add your API key:
        ```dotenv
        GOOGLE_API_KEY=YOUR_GOOGLE_API_KEY
        ```
4.  **Run the Streamlit App:**
    ```bash
    streamlit run main.py
    ```
5.  **Enter Stock Symbols:** In the sidebar, enter the stock symbols you want to analyze, separated by commas (e.g., AAPL, TSLA, GOOG).
6.  **Enter API Key:** Provide your Google Generative AI API key in the sidebar.
7.  **Generate Report:** Click the "Generate Investment Report" button.
8.  **View Analysis:** The application will display a comprehensive investment report, including market analysis, company-specific insights, and potential stock recommendations. An interactive chart showing the stock performance over the last 6 months will also be displayed.

## ⚙️ Dependencies

* `streamlit`: For creating the web application interface.
* `yfinance`: For fetching historical stock data and company information from Yahoo Finance.
* `agno`: An AI agent framework for building intelligent agents.
* `plotly`: For creating interactive stock price charts.
* `python-dotenv`: For loading environment variables (like the Google API key).
* `google-generativeai`: The official Google Generative AI library.

You can install all the necessary dependencies using the `requirements.txt` file.

## 🧠 How It Works

This application utilizes the `agno` library to create specialized AI agents that work together to provide investment insights:

1.  **Market Analyst:** This agent retrieves and compares the historical performance of the provided stock symbols over a 6-month period using Yahoo Finance data.
2.  **Company Researcher:** This agent fetches detailed information about each company, including its sector, market capitalization, business summary, and the latest news headlines, also using Yahoo Finance.
3.  **Stock Strategist:** This agent analyzes the market performance data and company-specific information to generate potential stock recommendations based on the provided instructions.
4.  **Team Lead:** This agent orchestrates the other agents, compiling their analyses and recommendations into a final, structured investment report for the user.

The application uses Google's `gemini-2.0-flash-exp` model for the AI agents, providing fast and efficient analysis. It also visualizes the stock price trends using interactive Plotly charts.

## ➕ Further Enhancements

* Implement more advanced technical analysis indicators in the stock charts.
* Allow users to specify different timeframes for stock performance analysis.
* Incorporate sentiment analysis of news articles to gauge market perception.
* Add risk assessment metrics for the recommended stocks.
* Allow users to save and track their analyzed stocks.

## 🙏 Contributing

Contributions to this project are welcome! Feel free to submit pull requests with bug fixes, new features, or improvements.
