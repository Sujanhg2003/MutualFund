# Project Title
## MutualFund Data Analysis using Python 
# Project Description
### Data Acquisition: I downloaded a dataset from a Kagggle data repository.
### Data Cleaning and Preprocessing:The dataset contains more missing values adn changes in data types.So I preprocessed a transformed a data to proper structure for analysis.
## Key Insights and Findings:
### 1.Performance Analysis
### 2.Risk Analysis
### 3.Fund Performance
### 4.Fund Manager Analysis
### 5.Risk-Return Tradeoff
### 6.Impact of Minimum SIP/Lump Sum Investment
# About Dataset
### Min sip: Min sip amount required to start.
### Min lumpsum: Min lumpsum amount required to start.
### Expense ratio: calculated as a percentage of the Scheme's average Net Asset Value (NAV).
### Fund size: the total amount of money that a mutual fund manager must oversee and invest.
### Fund age: years since inception of scheme
### Fund manager: A fund manager is responsible for implementing a fund's investment strategy and managing its trading activities.
### Sortino : Sortino ratio measures the risk-adjusted return of an investment asset, portfolio, or strategy
### Alpha: Alpha is the excess returns relative to market benchmark for a given amount of risk taken by the scheme
### Standard deviation: A standard deviation is a number that can be used to show how much the returns of a mutual fund scheme are likely to deviate from its average annual returns.
### Beta: Beta in a mutual fund is often used to convey the fund's volatility (gains or losses) in relation to its respective benchmark index
### Sharpe: Sharpe Ratio of a mutual fund reveals its potential risk-adjusted returns
### Risk level:
####  1->Low risk
####  2->Low to moderate
####  3->Moderate
####  4->Moderately High
####  5->High
####  6->Very High
### AMC name: Mutual fund house managing the assets.
### Rating: 0-5 rating assigned to scheme
### Category: The category to which the mutual fund belongs (e.g. equity, debt, hybrid)
### Sub-category : It includes category like Small cap, Large cap, ELSS, etc.
### Return_1yr (%): The return percentage of the mutual fund scheme over 1 year.
### Return_3yr (%): The return percentage of the mutual fund scheme over 3 year.
### Return_5yr (%): The return percentage of the mutual fund scheme over 5year.
### Number of instances: The dataset contains data on hundreds of mutual funds available in India.
## Disclaimer: The dataset is for educational and research purposes only. The data may not be 100% accurate and users should verify the data before making any investment decisions.

# Analysis:
# [![Interactive Plot](https://github.com/user-attachments/assets/34510ca9-7fa1-4084-826c-e6d2f4917b92)](https://sujanhg2003.github.io/MutualFund/sample_plot_1.html)

### The graph represents the distribution of sortino.
### The distribution is right-skewed (positively skewed), with a long tail extending to the right. This indicates that while most funds have Sortino ratios clustered around a central value, there are some funds with exceptionally high Sortino ratios.
### Range: The Sortino ratios in this dataset range from approximately -2 to 12, with the vast majority falling between 0 and 6.
### Frequency: The highest bar in the histogram corresponds to Sortino ratios between 3 and 4, with over 350 funds falling in this range.
### Outliers: There are very few funds with Sortino ratios above 6, which could be considered outliers or exceptionally well-performing funds in terms of risk-adjusted returns for downside risk.
### Negative Values: There's a small number of funds with negative Sortino ratios (below 0), indicating some funds that are underperforming relative to the risk-free rate when considering downside risk.
### Performance Implications: Given that higher Sortino ratios indicate better risk-adjusted performance, this distribution suggests that while most funds have moderate performance, there are a few standout performers with very high ratios.
# [![Interactive Plot](https://github.com/user-attachments/assets/b1ebfc29-9f51-4918-9f92-08df47c7c4eb)](https://sujanhg2003.github.io/MutualFund/sample_plot_2.html)






