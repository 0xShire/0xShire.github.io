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

