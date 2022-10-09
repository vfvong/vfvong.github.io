---
layout: post
title: How I Build a Very Short-Term Trading Strategy Based on the Squeeze Momentum
  Indicator
categories:
- Essays
tags:
- finance
- cryptocurrency
- trading
- squeeze-momentum
date: 2022-10-09 23:53 +0800
---
This is not my [main cryptocurrency trading strategy](/essays/2022/10/09/how-i-build-a-trading-strategy-based-on-ema-macd-and-rsi.html). I use a quarter of my assets for this strategy. It is applied to 15-minute bars.

First, we still use the EMA as an indicator to show up the current trend: When the price is above the EMA, it is in the **upward trend**; when the price is below the EMA, it is in the **downward trend**. We should look for a chance to place long orders in the upward trend, and place short orders in the downward trend.

Next, we use the [Squeeze Momentum](https://atas.net/atas-possibilities/squeeze-momentum-indicator/) indicator to look for an **entry point**: When the first grey dot appears, it's a signal of the entry point; If the histogram is above zero, we open a long position, and if the histogram is below zero, we open a short position.

We can also use the [ADX](https://support.atas.net/en/knowledge-bases/2/articles/8526-adx-di-di-) indicator as a **filter** for identifying the strong trend: If the DI+ is above the DI-, and the ADX is above 20, then the long signal can be trusted; If the DI- is above the DI+, and the ADX is above 20, then the short signal can be trusted.

As for the **stop loss** and **take profit** points, we can look for a suitable [support and resistance](https://www.investopedia.com/trading/support-and-resistance-basics/) point.

If the black dots appear again, but the take profit and stop loss points have not been triggered, then we can choose a more profitable time to close the position.
