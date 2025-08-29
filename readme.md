Project Title: Analysis of Trading Behavior vs. Market Sentiment

Overview

This project analyzes the relationship between trading behavior
(profitability, risk, volume) and market sentiment, using a Bitcoin
Market Sentiment Dataset (Fear & Greed Index) and Historical Trader
Data. The goal is to identify trends and patterns that could inform
smarter trading strategies.

Datasets Used

1\. \`fear_greed_index.csv\`: Contains historical data on the Bitcoin
Fear & Greed Index, including timestamp, value, classification (Fear,
Greed, Extreme Fear, Extreme Greed, Neutral), and date. 2.
\`historical_data.csv\`: Contains historical trading data with details
such as account, coin, execution price, size, side, timestamp, closed
PnL, etc.

Analysis Performed

1\. \*\*Data Loading and Preparation\*\*: Both datasets were loaded into
pandas DataFrames and merged based on date for alignment. 2.
\*\*Correlation Analysis\*\*: Calculated the linear correlation between
the Fear & Greed Index value and various trading behavior metrics
(Execution Price, Size Tokens, Size USD, Fee, Closed PnL). 3.
\*\*Sentiment-Based Analysis\*\*: Analyzed the average trading behavior
metrics across different Fear & Greed classifications to identify more
nuanced relationships. 4. \*\*Visualization\*\*: Generated
visualizations (scatter plots and bar charts) to illustrate the
relationships and trends. 5. \*\*Summarization\*\*: Summarized the key
findings, potential implications for trading strategies, and limitations
of the analysis.

Key Findings

\* Weak linear correlation was observed between the Fear & Greed Index
and the analyzed trading behavior metrics. \* Analysis by sentiment
classification revealed that \'Greed\' and \'Fear\' periods showed
higher average profitability compared to \'Extreme Greed\' and
\'Neutral\' periods. \* Trading volume (Size Tokens and Size USD) was
significantly higher during \'Extreme Greed\' periods. \*
Counter-intuitive finding regarding higher average execution prices
during \'Fear\' periods warrants further investigation.

Potential Implications for Trading Strategies

\* Considering sentiment in conjunction with specific trading metrics
and classifications may offer more valuable insights than relying on
sentiment alone. \* Strategies could potentially leverage the higher
profitability in \'Greed\' and \'Fear\' periods and manage risks during
high-volume \'Extreme Greed\' phases. \* Further analysis is needed to
understand the nuances of trading behavior within each sentiment
category and potential time lags.

Limitations

\* Focused primarily on linear correlations. \* Did not account for
potential time lags between sentiment changes and trading behavior. \*
Analysis was based on aggregated trading behavior, not individual trader
specifics. \* Lack of direct leverage data limited the assessment of
risk-adjusted returns.

Future Directions

\* Explore non-linear relationships and time-series analysis. \* Analyze
individual trader behavior. \* Seek additional data, particularly on
leverage.
