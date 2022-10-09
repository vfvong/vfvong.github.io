---
layout: post
title: How I Build a Trading Strategy Based on EMA, MACD, and RSI
categories:
- Essays
tags:
- finance
- cryptocurrency
- trading
- ema
- macd
- rsi
date: 2022-10-09 17:00 +0800
---
I currently build my mainly cryptocurrency trading strategy using three indicators [EMA](https://www.investopedia.com/terms/e/ema.asp), [MACD](https://www.investopedia.com/terms/m/macd.asp), and [RSI](https://www.investopedia.com/terms/r/rsi.asp). It is applied to the daily and 4-hour bars; the daily bars are used for spot trading, while the 4-hour bars are used for contract trading.

EMA is a type of [moving average](https://www.investopedia.com/terms/m/movingaverage.asp). One of main usages of the moving average indicator is to show up the current trend: When the price is above the moving average, it is in the **upward trend**; when the price is below the moving average, it is in the **downward trend**. We should look for a chance to place long orders in the upward trend, and place short orders in the downward trend.

(I apply the EMA instead of the [SMA](https://www.investopedia.com/terms/s/sma.asp) because that EMA places more weight on the recent data points. This property makes the EMA more sensitive to the momentum so that EMA is more suitable for short- and middle-term tradings.)

After judging the current trend, we should look for an **entry point**. When the MACD crosses above its signal line or the above-zero-histogram becomes longer, we place a long order. Similarly, we place a short order when the MACD crosses below its signal line or the below-zero-histogram becomes longer.

To strengthen the **reliability** of buy and sell signals, we can also consider the RSI indicator at the same time. When the RSI is between 50 and 70, we consider a buy signal to be reliable; when the RSI is between 30 and 50, we consider a sell signal to be reliable.

If we need to set a **stop loss point**, we can do this: for long orders, we can set the stop loss point to slightly lower than the nearest "wave bottom"; for short orders, we can set the stop loss point to slightly higher than the nearest "wave top".

Finally, the **exit point**: When the MACD crosses below its signal line, we close the long order; when the MACD crosses above its signal line, we close the short order.
