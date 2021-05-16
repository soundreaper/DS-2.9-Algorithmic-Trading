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
for the rest of the conclusions you can draw from the quanitative stock data. Links to the articles, blogs, and other GitHub repos I looked at can be found below:
- https://docs.quandl.com/
- https://www.freecodecamp.org/news/algorithmic-trading-in-python/
- https://medium.datadriveninvestor.com/machine-learning-models-for-market-beating-trading-strategies-c773ba46db66
- https://medium.datadriveninvestor.com/designing-market-beating-trading-strategies-utilizing-ml-models-61b8256065dc
- https://www.oreilly.com/content/algorithmic-trading-in-less-than-100-lines-of-python-code/
- https://blog.quantinsti.com/python-trading/
- https://github.com/gbeced/pyalgotrade
- https://github.com/nickmccullum/algorithmic-trading-python