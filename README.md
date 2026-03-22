# AI Stock Analyzer

A Python tool that pulls financial data for any public companies, compares key metrics side by side, and uses AI to generate a written analysis ranking them by overall financial strength.

## What It Does

Give it any set of stock tickers and it will:
1. Pull real-time company profiles, financial statements, and key metrics from the Financial Modeling Prep API
2. Display a comparison table of important financial data
3. Generate three charts — profit margins, return on capital, and debt burden
4. Use Google's Gemini AI to write a structured analysis that ranks the companies and explains why

## Example
```python
full_analysis(["AAPL", "MSFT", "GOOGL"])
```

This outputs:
- A financial comparison table with 17 key metrics
- Visual charts comparing margins, capital efficiency, and leverage
- An AI-written analysis identifying strengths, weaknesses, red flags, and an overall ranking

## Metrics Tracked

- Price, Market Cap, Sector
- Revenue, Net Income, EPS
- Gross Margin, Operating Margin, Net Margin
- Return on Equity (ROE), Return on Invested Capital (ROIC)
- EV/EBITDA, Earnings Yield
- Current Ratio, Net Debt/EBITDA

## How to Run

1. Click the badge below to open in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jackreichert11761/ai-stock-analyzer/blob/main/Stock_Analyzer_v1.ipynb)

2. Get a free API key from [Financial Modeling Prep](https://site.financialmodelingprep.com/developer/docs)
3. Paste your API key into the notebook where indicated
4. Run all cells
5. Call `full_analysis()` with any stock tickers

## Built With

- Python
- pandas
- matplotlib
- Financial Modeling Prep API
- Google Gemini AI (via google.colab.ai)

## Disclaimer

This tool is for educational purposes only. It is not financial advice. Always do your own research before making investment decisions.
