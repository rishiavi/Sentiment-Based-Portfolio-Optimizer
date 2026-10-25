# Sentiment-Based-Portfolio-Optimizer
Overview:
This Python pipeline applies natural language processing and quantitative finance concepts in order to optimize an investment portfolio based on market sentiment. It combines both mathematical mean-variance optimization and investor reaction to news.

Processes:
Python pipeline applies FinBERT to news articles via Alpha Vantage API for sentiment scoring across inputted stock universe.
CVXPY used to define and solve a constrained convex optimization problem, utilizing sentiment scores, portfolio risk (estimated through a rolling covariance matrix), and diversification constraints.
Constructed a backtest evaluating strategy performance against S&P 500 and ishares TOPT benchmarks, presenting metrics such as Sharpe ratio, cumulative returns, and alpha t-stat.

Next Steps:
The universe of stocks will be expanded, along with the sentiment to risk aversion ratio being tune during in-sample trading for higher alpha t-stat and lower p values, before moving on to longer 5 year out of sample backtests.
The optimization problem defined will be altered to implement dollar neutrality, encouraging increased short positions.
