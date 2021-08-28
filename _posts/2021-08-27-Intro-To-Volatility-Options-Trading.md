---
title: "Intro To Volatility Trading With Options"
date: 2019-08-27T19:04:30-05:00
categories:
  - blog
tags:
  - Options
  - Volatility
---

## Volatility And Derivatives
The rapid growth of digital assets has led to the creation of multiple crypto derivative markets, the most robust being those constructed around Bitcoin and Ethereum. Altcoins as well, however, have started to see futures markets and OTC option markets develop as traders have increasingly demanded tools to manage risk and capture yield.

For Bitcoin and Ethereum, analysis of these derivative markets can provide insight into likely future price movements. Similarly, they can provide clues as to how a trader should construct portfolios for risk management and alpha generation.

## Options
Options are financial instruments that are derivatives based on the value of underlying securities such as stocks. An options contract offers the buyer the opportunity to buy or sell—depending on the type of contract they hold—the underlying asset. Unlike futures, the holder is not required to buy or sell the asset if they choose not to.

- Call options allow the holder to buy the asset at a stated price within a specific timeframe.
- Put options allow the holder to sell the asset at a stated price within a specific timeframe.

Each option contract will have a specific expiration date by which the holder must exercise their option. The stated price on an option is known as the strike price. Options are typically bought and sold through online or retail brokers.

Contract periods longer than a week always expire on the last Friday of every month, while weekly options expire Friday each week. The number of expiration dates and strikes will vary based on a particular exchange's liquidity (or the amount of capital changing hands). 

Deribit, which hosts most of the digital asset options volume for Bitcoin and Ethereum, offers weekly options expirations for one month out, monthly expirations for one quarter out, and quarterly expirations one year out. Strike prices are less regular than expiration dates but always cluster around the spot price of the underlying asset. New strike prices will be added to the exchange if the price of the underlying asset changes significantly or if there is sufficient customer demand for a particular strike.

## The Greeks
![image](https://user-images.githubusercontent.com/87942881/131199847-e7db5acf-864a-4f5a-b56d-0cd817b049f2.png)

## Implied Volatility

Implied volatility is the parameter component of an option pricing model, such as the Black-Scholes model, which gives the market price of an option. Implied volatility shows how the marketplace views where volatility should be in the future.

Since implied volatility is forward-looking, it helps us gauge the sentiment about the volatility of a stock or the market. However, implied volatility does not forecast the direction in which an option is headed. In this article, we'll review an example of how implied volatility is calculated using the Black-Scholes model and we'll discuss two different approaches to calculate implied volatility.

- Make sure you can determine whether implied volatility is high or low and whether it is rising or falling. Remember, as implied volatility increases, option premiums become more expensive. As implied volatility decreases, options become less expensive. As implied volatility reaches extreme highs or lows, it is likely to revert to its mean.

- If you come across options that yield expensive premiums due to high implied volatility, understand that there is a reason for this. Check the news to see what caused such high asset expectations and high demand for the options. Keep in mind that after the market-anticipated event occurs, implied volatility will collapse and revert to its mean.

- When you see options trading with high implied volatility levels, consider selling strategies. As option premiums become relatively expensive, they are less attractive to purchase and more desirable to sell. Such strategies include covered calls, naked puts, short straddles, and credit spreads. 

- When you discover options that are trading with low implied volatility levels, consider buying strategies. Such strategies include buying calls, puts, long straddles, and debit spreads. With relatively cheap time premiums, options are more attractive to purchase and less desirable to sell. Many options investors use this opportunity to purchase long-dated options and look to hold them through a forecasted volatility increase.

![image](https://user-images.githubusercontent.com/87942881/131200154-635d744d-11cc-4f2a-9976-79022aae409f.png)
[Enlarge](https://user-images.githubusercontent.com/87942881/131200154-635d744d-11cc-4f2a-9976-79022aae409f.png)

## Realized Volatility
Realized volatility (RV) is the standard deviation of the market move, usually measured over a
trailing time series (30 days, 7 days). Realized volatility differs from implied volatility in that implied
volatility is based on the future expected price moves, derived from the pricing of options contracts,
while realized volatility is derived from the realized price action of the underlying asset.

![image](https://user-images.githubusercontent.com/87942881/131200239-c7ff8009-a868-4c68-b457-f4701ab2e29f.png)
[Enlarge](https://user-images.githubusercontent.com/87942881/131200239-c7ff8009-a868-4c68-b457-f4701ab2e29f.png)

## Realized / Implied Volatility Divergence
The divergence between implied volatility and realized volatility, coupled with other metrics, can help gauge market sentiment and directional propensity. It is generally the case that implied volatility is higher than realized volatility, as the expectation of volatility commands a premium in option markets for the uncertainty surrounding future price moves. When the divergence between realized volatility and implied volatility reaches statistically significant divergent levels, this can portend a change in the volatility regime, as volatility, in general, tends to oscillate within a range. Just as spot prices do not always go up, volatility does not always remain low, and this oscillation is precisely what allows derivative traders to generate alpha.

## Skew
Skew is the difference in implied volatility (IV) between out-of-the-money options, at-the-money options, and in-the-money options. The volatility skew, which is affected by sentiment and the supply and demand relationship of particular options in the market, provides information on whether fund managers prefer to write calls or puts.

When options traders are willing to pay more for downside strikes (puts) than upside strikes (calls) there is said to be a bearish skew in markets. Investors can use these metrics to anticipate future price movements, or to take contrarian positions, betting against skew and selling “overpriced” option premia.

Trading around Skew typically involves trading a spread in which the long option is closer to the money, with lower implied volatility, and the short option is traded further out of the money where higher implied volatility exists. The goal is to capture the spread in volatility as skew normalizes and closes the volatility gap. Non-standard ratio spreads are a good way to trade around skewness and capitalize on the ebb and flow of volatility

![image](https://user-images.githubusercontent.com/87942881/131200315-40da80ca-783a-4536-b978-3a48abac0411.png)
[Enlarge](https://user-images.githubusercontent.com/87942881/131200315-40da80ca-783a-4536-b978-3a48abac0411.png)

## Put / Call Ratio
The Put to Call ratio is the ratio of the trading volume of put options to call options and is used as an indicator of investor sentiment in the markets. When the value exceeds 1, it indicates that more puts are being purchased and traders are expecting a move lower. Conversely, a reading below 1 would indicate that traders are net bullish on the future price and are purchasing more calls.

Monitoring this ratio provides some insight into the overall sentiment of option market participants, and although it may not always provide actionable trade execution, it can provide instruction on how to manage a larger portfolio, and longer duration option positions.

 As the Put/Call ratio enters statistically high and low ranges, ranked across previous cycles, these open interest levels may serve as warning flags that conditions could fluctuate, oscillating between stability and volatility

One way to interpret the put-call ratio is to say that a higher ratio means it's time to sell and a lower ratio means it's time to buy. That's because when the ratio is high it suggests that people are either expecting or protecting more readily against a future decline in the price of the underlying. A put-call ratio between 0.5 and 1 is considered a sideways trend in the markets.

Some also view the put-call ratio as a contrarian indicator. Traders know that derivatives are used to do more than place bets; they are used as hedges and insurance. If there's a lot of insurance being placed to the sell side, it means traders are worried about prices falling.

Some traders buy when the put-call ratio is above 1, meaning the market is out of balance to the sell side, and sell when the put-call ratio is below 1, meaning the market is out of balance to the buy side. These traders are looking to make money on the correction. The interpretation of the ratio is left to the analyst's or trader's investment philosophy.

![image](https://user-images.githubusercontent.com/87942881/131200637-3b479153-dfeb-4713-8654-ab358230edd4.png)
[Enlarge](https://user-images.githubusercontent.com/87942881/131200637-3b479153-dfeb-4713-8654-ab358230edd4.png)

## Trading Volatility 
By combining data from the derivatives markets, you can take advantage of market structure and better position protective positions or speculative long positions to simultaneously reduce costs (premium paid) and anticipate volatility. 

While any single indicator is likely inadequate to make definitive adjustments to the portfolio, using the above-mentioned derivative metrics like Implied Volatility, Skew, and Put/Call Ratios together provide a more holistic approach to building both long and short volatility portfolios.

## Long & Short Volatility Positions
Consider markets amid a statistically “low volatility” environment relative to previous volatility cycles. During low volatility conditions it is not beneficial to maintain short volatility positions—the risk/reward is dangerous. Volatility premiums are generally too low to make it worth the risk to be a seller. 

These environments are often better managed using options spreads to offset volatility exposure and express delta. Short delta (expected move down) in a low volatility environment can be expressed by a Long Put Spread (PS), Naked Put, or Short Call Spread (CS).  All of these are preferable to selling naked calls. 

If the market is in a period of extremely low volatility and option premiums become statistically inexpensive, you should look to enter long volatility strategies.  Strangles and Long Iron Condors are ways to capture the future price volatility when it returns. Long option positions in a low volatility environment will benefit from directional moves (Delta Δ) as well as expansion in Vega (ν) and Gamma (Γ).

![image](https://user-images.githubusercontent.com/87942881/131200747-5ba2c9d7-c8e8-40f9-a97b-d8710eeb4003.png)

![image](https://user-images.githubusercontent.com/87942881/131200755-aea7575e-def7-4793-9712-0028287f682f.png)

## Hedge Positions vs. Speculative Positions
The responsibility of maintaining hedge positions to offset core portfolio Delta is generally non-negotiable. While the delta ratio of a derivative portfolio vs. spot can vary within a range of targeted short deltas, the deltas of the hedge vs. core portfolio should always remain inversely correlated, or protective into tail events. 

Speculative positions, however, can be far more dynamic with regard to the total holding time, profit targets, and delta expression.

## Structuring A Low Volatility Portfolio
![image](https://user-images.githubusercontent.com/87942881/131200896-d337d504-1f31-4ad4-883b-4f6b5d2e849d.png)
[Enlarge](https://user-images.githubusercontent.com/87942881/131200896-d337d504-1f31-4ad4-883b-4f6b5d2e849d.png)

The above market conditions indicate a tightening of the price range with declining volatility.  These conditions encourage long premium positions as option prices compress.

The following are sampled Put Spreads for low volatility conditions.  At the time of writing, price of the underlying is $48,864.

Long $49,000 x $44,000 Put Spread 1x1
- Max Risk: $2,154.47
- Max Reward: $2,845.53
- R-Multiple: 1.32
![image](https://user-images.githubusercontent.com/87942881/131201022-6f3dd694-5df9-43bb-844f-c2934901007e.png)
[Enlarge](https://user-images.githubusercontent.com/87942881/131201022-6f3dd694-5df9-43bb-844f-c2934901007e.png)

Long $47,000 x $44,000 Put Spread 1x1
- Max Risk: $1,230.40
- Max Reward: $1,769.60
- R-Multiple: 1.44
![image](https://user-images.githubusercontent.com/87942881/131201052-2dd40101-5fc4-46a8-b97e-a224597fb023.png)
[Enlarge](https://user-images.githubusercontent.com/87942881/131201052-2dd40101-5fc4-46a8-b97e-a224597fb023.png)

Long $45,000 x $43,000 Put Spread 1x1
- Max Risk: $719.06
- Max Reward: $1,280.94
- R-Multiple: 1.78
![image](https://user-images.githubusercontent.com/87942881/131201083-fda6377e-dbed-4bb6-9027-88ce3eea82d1.png)
[Enlarge](https://user-images.githubusercontent.com/87942881/131201083-fda6377e-dbed-4bb6-9027-88ce3eea82d1.png)

Long $42,000 x $40,000 Put Spread 1x1
Max Risk: $431.13
Max Reward: $1,568.87
R-Multiple: 3.64
![image](https://user-images.githubusercontent.com/87942881/131201104-99b58957-3f57-4c75-99a5-4be8a11ff25c.png)
[Enlarge](https://user-images.githubusercontent.com/87942881/131201104-99b58957-3f57-4c75-99a5-4be8a11ff25c.png)

As strike price moves further (OTM) from the index price, the cost of each spread and probability of profit (PoP) decreases while the risk / reward profile increases.
Now let's look further out in duration:

September 30 Option Chain - 34 DTE Long $45,000 x $40,000 Put Spread 1x1
- Max Risk: $1,732.76
- Max Reward: $3,267.24
- R-Multiple: 1.89

![image](https://user-images.githubusercontent.com/87942881/131201200-052ce036-ebbc-4c0b-9103-b1a5a145a9a9.png)
[Enlarge](https://user-images.githubusercontent.com/87942881/131201200-052ce036-ebbc-4c0b-9103-b1a5a145a9a9.png)

This spread takes advantage of a low volatility environment and provides asymmetric downside risk mitigation. 
