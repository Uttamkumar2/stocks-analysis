# Stock Analysis

Steve, A fresh graduated with finance degree, His parents are so proud that they wanted to become his first client, Steve’s parents are passionate about green energy, but they have not done much research in green energy stocks, they decide to invest in DAQO new Energy Corp, its ticker symbol is DQ. Steve promised to look into DQ Stocks for his parents but he is concern about diversifying his parents’ funds. He wants to analyze hand full of other green energy stocks as well in an automated way with help of excel. 

## Overview of Project

In the 1st phase of analyzing, it was working well for handful of stocks but it might not work for thousands of stocks. Now to do a little more research for his parents, Steve wanted to expend the dataset to include the entire stock market over the last few years. Although code from 1st phase of implementation would work but it may take a long time to execute.
So, the purpose of this analysis is to Modify or refactor code to support entire stock market data for last few years and most important in less time than 1st attempt of analyzing of dozens of stocks data. In the process of refactoring, it’s going to be absolutely no change in output but by taking few steps out and by changing approach, it using less memory and making easier for future users to read. 

## Results

By looking at the Dozens for stocks between year 2017 and 2018 , its looks like ticker “ENPH” & “RUN” stock consecutively given +ve result, In Process of refactoring code, we remove nested loops to single loop and create List variable (Array) like tickerVolumes , tickerStartingPrices tickerEndingPrices correspondingly to keep sum of total volume for given ticker , similarly tickerStartingPrices & tickerEndingPrices to keep beginning of stock price and end of stock price, and its access by its index count, indexcount increment happens only when next ticker is not equal to current tinker,  this more like in-memory processing resulting around 18% better performance for 2017 stocks and 16% better performance in 2018 stock data. Actual Outputs are given below.


![VBA_Challenge_2017](https://user-images.githubusercontent.com/91766890/138580159-dc2ec4f4-ca39-404e-a2fd-fcd1016657ac.png)            ![VBA_Challenge_2018](https://user-images.githubusercontent.com/91766890/138580177-61a0d1a2-28f0-4f03-812b-05d12deec454.png)

## Summary

Over all after refactoring its improved performance, code looks more organized and readable and user friendly and above all it improves overall design. With so many of advantages it comes with some advantages also but these dis-advantages depending upon criticality and dependencies, it makes cause to introduce new bug and it’s risky when application id too big.
