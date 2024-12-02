# Project Overview

This project consolidates financial, fundamental, and analyst recommendation data to provide a comprehensive dataset for analyzing stock performance and company metrics. The dataset integrates various sources, cleans and transforms the data, and outputs quarterly-level aggregated information.

## Directory Structure
- **data/**: Contains the raw and intermediate CSV files used for data processing.
  - `analyst_data.csv`: Contains analyst ratings and recommendations.
  - `constituents_data.csv`: Holds stock-level market data.
  - `fundamental.csv`: Includes company-level fundamental financial metrics.
  - `fundamental_global.csv`: Global version of the fundamental dataset.
  - `russel_1000_growth.csv`: Russell 1000 growth index dataset.
  - 
- **data_builder.ipynb**: The main Jupyter Notebook used for data processing and merging.

## CSV Columns in `final_merged_data.csv`
The final dataset includes the following columns:

### Stock Data
- **Company Name_x**: The company name.
- **TICKER**: The stock's ticker symbol.
- **Quarter**: The quarter of the data record (e.g., Q1 2023).
- **Price**: Average stock price for the quarter.
- **Total Ret**: Total return, including dividends, for the quarter.
- **Price Ret Ex-Dividend**: Average price return excluding dividends.
- **Weighted Mkt Return**: Market-cap-weighted return for the quarter.
- **Volume**: Total trading volume during the quarter.
- **Dividend**: Total dividend paid during the quarter.
- **Price Low**: Lowest stock price during the quarter.
- **Price High**: Highest stock price during the quarter.
- **Shares Outstanding**: Average number of outstanding shares during the quarter.

### Financial Metrics
- **Excess Return**: Return in excess of the market benchmark.
- **Mkt Cap**: Market capitalization (Price × Shares Outstanding).
- **Price Growth Rate**: Quarter-over-quarter price growth rate.
- **Quart Rev**: Quarterly revenue in USD.
- **Quart NI**: Quarterly net income in USD.
- **Equity**: Total shareholder equity.
- **Liabilities**: Total liabilities of the company.
- **Revenue**: Total revenue for the quarter.
- **Industry Code**: Industry classification code.
- **Asset**: Total company assets.
- **Current Asset**: Current assets of the company.
- **EPS**: Earnings per share (Net Income / Shares Outstanding).

### Growth and Ratios
- **Revenue Growth**: Quarter-over-quarter revenue growth rate.
- **Earnings Growth Rate**: Quarter-over-quarter EPS growth rate.
- **P/E Ratio Annual**: Annualized price-to-earnings ratio.
- **P/E Ratio Quarter**: Quarterly price-to-earnings ratio.

### Analyst Ratings
- **Mean Recommendation**: Average analyst recommendation (1 = strong buy, 5 = strong sell).
- **Median Recommendation**: Median analyst recommendation.
- **Recommendation StdDev**: Standard deviation of analyst recommendations.
- **Number of Recommendations**: Total number of analyst recommendations.
- **Number of Upgrades**: Count of analyst upgrades during the quarter.
- **Number of Downgrades**: Count of analyst downgrades during the quarter.
- **Buy Percentage**: Percentage of buy recommendations.
- **Sell Percentage**: Percentage of sell recommendations.
- **Hold Percentage**: Percentage of hold recommendations.
- **Rating**: SP Quality Index.

## Usage
The dataset can be used for:
1. **Stock Analysis**: Evaluate stock performance using metrics like returns, growth rates, and analyst sentiment.
2. **Factor Research**: Identify key drivers of stock price and earnings growth.
3. **Machine Learning Models**: Prepare data for predictive analytics or financial modeling.
4. **Backtesting**: Test trading strategies using historical financial and sentiment data.

## Next Steps
- Enhance the dataset with additional global financial data.
- Refine the merging process to reduce missing values and ensure ticker consistency.
- Explore advanced analytics using the combined dataset.


### Final Report
https://docs.google.com/document/d/1L8ZmcgMK6do0M8QaQucsRR35Q7UVqS1rUXyujdFbd6M/edit?usp=sharing