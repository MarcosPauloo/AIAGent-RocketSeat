
# Stock Market Analysis with AI

This project is a comprehensive tool for analyzing stock prices and market news using AI. It combines data from Yahoo Finance and web search results to provide detailed insights into stock trends, news sentiment, and overall market conditions. The results are compiled into a concise newsletter format, providing actionable insights for traders and investors.

## Features

- **Stock Price Analysis**: Fetches historical stock prices from Yahoo Finance and analyzes trends.
- **Market News Summary**: Searches for the latest news about a specific stock and analyzes the sentiment and trend.
- **Newsletter Generation**: Compiles the analysis into a well-structured newsletter format, highlighting key points and predictions.
- **Interactive Web Application**: Built with Streamlit, allowing users to input stock ticker symbols and receive a detailed analysis report.

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/stock-market-analysis-ai.git
   cd stock-market-analysis-ai
   ```

2. **Install Dependencies**
   Make sure you have Python 3.8 or higher installed. Then, install the required packages using pip:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up Environment Variables**
   Create a `.env` file in the root directory of the project and add your OpenAI API key:
   ```plaintext
   OPENAI_API_KEY=your_openai_api_key_here
   ```
   Ensure that the `.env` file is included in your `.gitignore` to prevent it from being uploaded to GitHub.

## Usage

To run the application locally, use the following command:

```bash
streamlit run app.py
```

This will start a Streamlit web application where you can enter a stock ticker symbol and receive a detailed analysis.

### Example

1. **Enter the Stock Ticker**: Input the ticker symbol (e.g., `AAPL` for Apple Inc.) in the sidebar form.
2. **Run Research**: Click the "Run Research" button to execute the analysis.
3. **View Results**: The application will display the final report, including stock price trends, market news summaries, and a newsletter.

## How It Works

1. **Yahoo Finance Tool**: Fetches the stock price history for the past year.
2. **News Analysis**: Uses the DuckDuckGo Search tool to find relevant news articles about the stock and evaluates sentiment.
3. **Report Generation**: Combines the price analysis and news summary to generate a well-structured report in markdown format.

## Project Structure

- `app.py`: The main application file containing the Streamlit web interface and logic for generating stock analysis reports.
- `crewai.py`: The core logic for defining agents and tasks using the CrewAI library.
- `.env`: Environment file (not included in the repository) where the OpenAI API key is stored.

## Dependencies

- [Streamlit](https://streamlit.io/) - For building the web application.
- [yfinance](https://pypi.org/project/yfinance/) - To fetch stock data from Yahoo Finance.
- [langchain](https://langchain.com/) - To interact with language models.
- [dotenv](https://pypi.org/project/python-dotenv/) - For loading environment variables.

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License.

## Acknowledgments

This project was developed based on the concepts and ideas presented during the "IA na prática" event by RocketSeat.

---

### Disclaimer

This tool is for educational purposes and does not constitute financial advice. Always conduct your own research and consult with a professional before making any investment decisions.
