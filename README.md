# Algorithmic Trading with Python

## What is this project about?
This project is about using Python to analyze Stock Market data and use said date to predict gain or loss to trade stocks effectively. For the minimum viable product, there would have to be data about any given stock and
a functioning trading algorithm that gives the user some type of positive return on a given stock. There would also have to be some way to test the trading algorithm without a user actually putting real money into it; some
way to backtest the algorithm. The value behind being able to do this is building a trading algorithm and optimizing it effectively to trade real world money. We would be able to learn about all the different types
of events and signals that affect stock prices and observe these changes to the market.

## Goals/Plan
- Analyze quanitative stock data from a stock from a large company
- Generate some visuals for given stock
- Apply common financial analysis on given stock
- Build a trading algorithm using analysis
- Backtest the trading strategy
- Calculate metrics to see how effective trading strategy is

## Stretch Goals?
- Test 3-4 other stocks
- Test another trading strategy
- Use metrics to create event driven trading algorithm (VERY STRETCH)

## 6 Week Project?
It will take time to analyze the stock, develop the trading algorithm, and back test the algorithm. This is my first time doing such a project related to Data Science so I will have to do some reading about trading algorithms
and proper financial analysis. I also need to find some way to pull stock data into Jupyter Notebook so I can use it for analysis. In terms of compute and storage resources, all the files will be stored locally on my computer
and I will keep note of the total file size after I finish this project. It will be updated below:

TOTAL PROJECT FILESIZE: 2.89 MB

## Implementation & Results
In terms of implementation, there were not many assumptions to be made besides whether the trading algorithm would work or not on a given stock. Of course based on the results, the trading algorithm did work. Results are contained
within the notebook itself after the section about backtesting. It mentions how much money the strategy used made via backtesting and goes over metrics that could be used to improve the results further. There were no real problems
when it came to testing the algorithm and doing analysis on the stock of choice. There was, however, an issue when trying to collect data. The Python module I was using actually had issues getting data from Yahoo! Finance and I had
to install another module that allowed the first one to function properly. This was fixed with a simple Google search so it wasn't a large issue.

## How to Run Project
### Step 1:
Clone this repository.
```git
git clone https://github.com/soundreaper/DS-2.9-Algorithmic-Trading.git
```
### Step 2:
Navigate to the folder via terminal and run:
```bash
jupyter notebook
```
### Step 3:
Once the file system opens in your browser, open the notebook contained within the folder.

## Summary of Research
Based on my research, many of the resources I looked at stated the most important part of an algorithmic trading project is coming up with a trading algorithm. It's the most crucial part of the project and serves as the basis
for the rest of the conclusions you can draw from the quanitative stock data. Summaries of articles used for research
can be found below:

- https://medium.datadriveninvestor.com/machine-learning-models-for-market-beating-trading-strategies-c773ba46db66
- https://medium.datadriveninvestor.com/designing-market-beating-trading-strategies-utilizing-ml-models-61b8256065dc
- https://www.freecodecamp.org/news/algorithmic-trading-in-python/
- https://www.investopedia.com/articles/active-trading/101014/basics-algorithmic-trading-concepts-and-examples.asp
- https://www.trality.com/blog/algorithmic-trading
- https://medium.com/oreillymedia/algorithmic-trading-in-less-than-100-lines-of-python-code-b4a4b159a485

### Articles 1-3:
The goal of this project would be to use machine learning techniques to predict short term movements in the stock market and “swing trade” based on this information. I want to be able to predict what a stock might do within 10 days using my machine learning models. The potential value of this project would be to develop an actually functioning algorithm trading model that would allow me to trade stocks in the real world and grow my money. I would have to collect data but I have an idea of what the data would look like. Each row in the dataset would be each day for each stock. I also want to see if I can target between 50-100 stocks and the last 5 years of trading for each of those stocks. If there are 250 trading days in a year this would be approximately 100,000 rows of data. I’d like to keep this project under ~50 mb if possible.

Others have approached this problem in a similar way to how I described. They collected data in a very similar fashion but how they processed it might differ. I have to process the data to make predictions about whether the stock value will increase or decrease. I was considering using a momentum-based Simple Moving Average Crossover (SMAC) strategy to make my predictions for my project. I think I could do this entire project on my laptop but I will use my desktop PC or Google Collab if I need the extra horsepower. I would have to learn a little more about what data I can obtain from the stock market. I am also interested in learning if there are other more complicated trading strategies that are potentially more profitable.

### Article 4:
Algorithmic trading uses a computer program to follow a defined set of instructions to place a trade. The benefit of this is that, in theory, this type of trading can generate profits at speeds or frequencies that would be impossible for a human trader. A simple trading ruleset that one could follow would be to buy fifty shares of a stock when the fifty day moving average goes about the two hundred day moving average. Then, the individual could sell the stock when the fifty day moving average goes below the two hundred day moving average. Using this ruleset, a computer program could automatically monitor the stock price and place the buy and sell orders when the conditions are met. The trader does not have to be present or put the orders in manually. Some other benefits to algorithmic trading are that trades are generally executed at the best possible prices, they are usually instant and accurate, there are reduced transaction costs, and there are much more reduced chances of error due to human psychological factors.

### Article 5:
Python is a programming language that is great for algorithmic trading. It is used by institutions and investors alike every day for a range of purposes. Python code is readable and accessible and generally easy to learn so it is the best choice for getting into algorithmic trading. There are several libraries such as Pandas that Python users can use for easier data visualization and sophisticated statistical analysis. There are also powerful machine-learning algorithms that can do predictive analysis using Python-based solutions suchs as Scikit of PyBraing. Trality is a code-editor that allows users to build a trading bot using a browser-based Python Bot Code Editor. It allows for users to track key metrics automatically, backtest, fine-tune a strategy, add exchanges, and for virtual and live trading. This could be useful to my project to see how to potentially create a trading algorithm or for how to fine-tune my algorithm.

### Article 6:
Algorithmic trading refers to the computerized, automated trading of financial instruments based on some algorithm or rule with little to no human intervention during trading hours. Any type of financial instrument can be traded in such a fashion. The barrier to entering algorithmic trading is quite low and now just about anyone with a laptop and internet connection can do it. The strategy presented in this article is a time series momentum strategy which assumes that a financial instrument that has performed well or poorly will continue to do so. The platform of choice here is called Oanda and it allows a user to trade a variety of leveraged contracts which allows for direction bets. All the data will also be provided by Oanda. Python is the programming language of choice. The first step is to set up an Oanda account so that the user can work with the Oanda API. Next, we grab the data using the Oanda API and then we use NumPy to generate the mean log for given time intervals. Then we generate the positions generated in the previous step by the market returns to determine the gross performance of the strategy. A graph will be generated which shows which position is the best to use with the provided strategy. Lastly, we will go back to the Oanda API to use the library to do automated trading with the picked strategy. Running this will show the simulated trading within Oanda and show the gains or losses of the chosen strategy.