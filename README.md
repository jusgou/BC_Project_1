# PROJECT OVERVIEW

![RoboAdvisor](Images/GettyImages_RoboAdvisor.png)

## HUMAN ROBOMYSTIC: Automated Investing that Feels Human
---

##  COLLABORATORS
- Coney Dacanay
- Dipendra Shastri
- Justin Gouin 
- Sherin Solomon
- Yu Wang

---
##  Please review the Master_Final

---
##  SUMMARY


Investing in the stock market may seem to be intimidating and complicated, this project proposes an avenue to simplify and automate the process of choosing among the thousands of publicly-traded stocks in the U.S. market with the consideration of company performance and the investor’s risk tolerance. 

The core stock selection process will be using more than 20 years of historical company stock data, beginning from year 2000 until the current day. Also, to streamline the complexity of various investing strategies, this project will mimic the strategy of an index investor by using S&P 500 Index (SPY) as its baseline. SPY data will be used for comparison on company information and performance across all portfolios that will be recommended after the financial analysis.  

---
## OBJECTIVES

- To create a stock-allocating model that provides clients with a list of publicly-traded stocks based on their personal and risk profiles.
- To allow customers to build their own portfolio of equity stocks through exploring among recommended stocks and adjusting the weightings/ratios in order to maximize potential earnings. 
- To present stock performance forecasting for finalized portfolios.

---
## METHODOLOGY

**1. Client Onboarding & Know Your Client (KYC)**

The YAML (YAML Ain’t Markup Language) module was utilized, as recommended by one of our mentors, to configure, store, and transmit client’s data; prospective clients will be filling out a KYC form. Although the KYC format used for this project only covers few basic data points and does not meet the Canadian KYC and Anti-Money Laundering (AML) requirements, incorporating the YAML file will help in the process of relating the client’s risk tolerance taken from the KYC form with the risk level of various publicly-trading companies based on chosen financial criteria. 

**2. Data Exploration**

Aside from the information that will be provided by clients through the KYC YAML forms, majority of the working data used in this project were captured from Yahoo! Finance with the combination of these sources and processes:
- Data scraping from Yahoo! Finance website
- Python modules such as yfinance and yahoofinancials


**3. Company Overview & Benchmarking**

As an initial report presented to clients, the company information dataframe serves as a summary of recommended companies to invest in, which risk levels match the risk tolerance of the client. This table  shows fundamental company information as well as an overview of company performance of each recommended company side-by-side with each other and along with the project’s main exchange-traded fund (ETF) benchmark, the S&P 500 (SPY). Clients are encouraged to review and compare these information for them to decide on the initial mix of stocks to build their portfolio according to their preference. 

**4. Financial Analysis & Portfolio Allocation Proposal**

To take a deeper look at company performance, statistical analysis of the historical stock data will be performed with the intention of organizing the stocks into their respective risk level (low, mid, high) or category based on predetermined criterias. 

Each stock’s risk level will be categorized based on these three financial statistical criteria which will be matched with the client’s risk tolerance:
- Annualized standard deviation [Low: <2 | Mid: 2-5 | High: >5];
- Sharpe ratio [Low: 1-5 | Mid: 6-10 | High: >10]; and 
- P/E Ratio [Low: <10 | Mid: 10-20 | High: >20].

After narrowing down the list of the matched stocks, clients can create the breakdown of each stock within their portfolio.

**5.Client Recommendations**

 The customers are categorized based on Qualifiers and Assumptions. At this stage in our understanding of data analysis, we have added various human elements to assign the data.

Our program makes recommendations to our customers based on its interpretation of their KYC information and recommends a portfolio.

In future iterations of our project, these recommendations will be taken as the baseline on which customers can build. They will be able to interact with and change their portfolios to explore other options, which will include our visualizations.

As our company name suggestions, the automated system provides suggestions, but control over the outcome remains with the humans.

---
## POTENTIAL FEATURES AND PROJECT EXPANSION

- **Contingency Planning**

What happens to one’s investments in the event of an economic crisis, a catastrophe, and/or a pandemic? Forecasting portfolio performance on situations leading to extreme volatility (Sharpe Ratio).

- **User interface**

To further utlize the 20-year historical data, it would be nice to include a slider that allows the user to choose the number of historical years to incorporate into projections.

- **Flexible Investment Thresholds**

 Allow potential clients to invest in each stock from $20 to possibly $20 million to maximize the capability of clients in placing weights of their investments into different stocks.

- **Online Stock Trading**

Integrate an automated trading program that allows online buying and selling when clients are satisfied with the selected portfolio.

---
## GENERAL REFERENCES

- https://pypi.org/project/yahoo-finance/
- https://pypi.org/project/FundamentalAnalysis/
- https://codingandfun.com/comparing-industry-profitability-ratios-with-python/
- https://corporatefinanceinstitute.com/resources/knowledge/finance/sharpe-ratio-definition-formula/
