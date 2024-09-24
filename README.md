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

### The graph represents Performance Analysis,Returns over 1, 3, and 5 Years.Return variability increases with the time horizon, as shown by the expanding box sizes from 1 to 3 to 5 years.
### Median returns are highest for the 3-year period, followed by 5-year, then 1-year.3-year returns have the widest interquartile range, suggesting more diverse performance over this period.5-year returns are more concentrated, implying more consistent long-term performance across funds.

# [![Interactive Plot](https://github.com/user-attachments/assets/bc4bb582-cb61-4de0-b30f-91084e717557)](https://sujanhg2003.github.io/MutualFund/sample_plot_3.html)
### The above graph represents a  Risk vs. Return (3-Year).There's a general positive correlation between risk (standard deviation) and return.Most funds cluster in the lower risk range (0-20 standard deviation) with returns between 0-40%.A few high-performing outliers show exceptional returns (60-70%) with moderate risk.Some funds show high risk with relatively low returns, indicating poor risk-adjusted performance.The relationship isn't perfectly linear, suggesting factors beyond risk influence returns.

# [![Interactive Plot](https://github.com/user-attachments/assets/bd69330c-1338-4c71-8c33-a7e22f36c73a)](https://sujanhg2003.github.io/MutualFund/sample_plot_4.html)
### The above visuals represents Distribution of Risk Levels."Very High" risk level is the most common category by far."Low to moderate" and "Moderate" risk levels have similar, moderate frequencies.There are relatively few funds in the "High" risk category."Low risk" funds are less common than moderate risk options.The distribution skews heavily towards higher risk levels, indicating a prevalence of more aggressive fund options.

# [![Interactive Plot](https://github.com/user-attachments/assets/dcff4c2e-d61e-4929-b51f-f3d0519105da)](https://sujanhg2003.github.io/MutualFund/sample_plot_5.html)
### There's a general trend of decreasing expense ratios as fund size increases.Smaller funds show a wider range of expense ratios, from very low to very high.Larger funds (above 20,000 fund_size_cr) tend to have lower expense ratios, mostly below 1.5%.Very high risk funds (purple) seem to be more prevalent among smaller fund sizes.Low risk funds (blue) appear to cluster in the lower fund size range with varying expense ratios.

# [![Interactive Plot](https://github.com/user-attachments/assets/41ec0e82-9887-4679-8bd3-36d5dd555940)](https://sujanhg2003.github.io/MutualFund/sample_plot_6.html)

### The graph represents the Distribution of Fund Categories.Equity funds are the most common category, followed closely by Debt funds.Hybrid funds form a significant but smaller portion of the overall fund offerings.There's a moderate number of "Other" category funds, suggesting specialized or niche offerings.Solution Oriented funds are the least common category.The distribution shows a clear preference for pure equity or debt funds over mixed or specialized options.

# [![Interactive Plot](https://github.com/user-attachments/assets/2eb9c506-7ad7-4151-9f0c-a2401c05ed63)](https://sujanhg2003.github.io/MutualFund/sample_plot_7.html)
### The bar graph represents Top 10 Fund Managers by Average 3-Year Returns.Vasav Saigal is the top-performing fund manager with an average 3-year return of over 50%.There's a significant gap between the top performer and the others, with Samir Rachh in second place at around 47% return.The top 3 managers (Vasav Saigal, Samir Rachh, and Vaibhav Dusad) all achieve returns above 45%.There's a gradual decline in performance from the top to the bottom of the list.Even the 10th ranked manager, Rohit Singhania, achieves a respectable average 3-year return of about 35%.

# [![Interactive Plot](https://github.com/user-attachments/assets/73fcafda-9dee-4bcb-ac5d-ff18259c4fc7)](https://sujanhg2003.github.io/MutualFund/sample_plot_8.html)
### The scatter plot represents Sharpe Ratio vs 3-Year Returns.There's a clear positive correlation between the Sharpe Ratio and 3-Year Returns, indicating that higher risk-adjusted returns generally correspond to higher absolute returns.The relationship is not perfectly linear, suggesting that factors beyond risk-adjusted performance influence returns.A few funds stand out with exceptionally high returns (60-70%) and high Sharpe Ratios, representing the best risk-adjusted performances.There's a wide dispersion of returns for any given Sharpe Ratio, particularly in the middle range.Many funds cluster in the lower return range (0-10%) across various Sharpe Ratios, suggesting a significant number of underperforming funds regardless of their risk-adjusted metrics.The density of points increases as the Sharpe Ratio increases, indicating that more funds achieve higher risk-adjusted returns.

# [![Interactive Plot](https://github.com/user-attachments/assets/828e13f2-8e67-4028-b879-8786d1796aad)](https://sujanhg2003.github.io/MutualFund/sample_plot_9.html)
### The visuals represents Impact of Minimum Investment on Returns.There's no clear correlation between minimum investment amount and returns, suggesting that higher minimum investments don't necessarily lead to better performance.The highest returns are achieved by funds with minimum investments in the 100-10,000 range, indicating that top-performing funds are accessible to a wide range of investors.There's a wide dispersion of returns for each minimum investment level, particularly in the 100-1,000 range.
### SIP (Systematic Investment Plan) options tend to have lower minimum investment requirements compared to lump sum investments.Some funds with very low minimum investments (around 10) still achieve competitive returns, making them attractive for small investors.                                                              The density of funds is highest in the 100-1,000 minimum investment range, suggesting this is a sweet spot for fund offerings.There are fewer funds with very high minimum investments (10,000+), and their performance doesn't appear to be consistently superior.






