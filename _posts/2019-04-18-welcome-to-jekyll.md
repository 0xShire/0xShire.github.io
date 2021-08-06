---
title: "Welcome to Jekyll!"
date: 2019-04-18T15:34:30-04:00
categories:
  - blog
tags:
  - Jekyll
  - update
---

##What are MOVE contracts?
MOVE contracts are a volatility derivative offered by FTX.  Each MOVE contract expires to the absolute value of the amount the underlying asset (BTC) moved on the traded timeframe.  If BTC opens the trading day at $35,000 and closes the day at $36,500, the daily BTC MOVE contract will expire at a value of $1,500.  If BTC falls from $36,500 to $33,000 the next day, for example, that daily MOVE contract would expire to $3,500.

##MOVE Contract Types
MOVE contracts are offered in three varieties on FTX—daily, weekly, and quarterly.
Daily MOVE contracts expire to the absolute value of the distance BTC has moved from open to close in a single day.  The ticker for each daily MOVE contract is BTC-MOVE-[EXPIRY].  For example, BTC-MOVE-0805 is the daily BTC MOVE contract expiring at the daily close of August 5th. 

Weekly MOVE contracts expire to the absolute value of the distance BTC has moved from open to close in a single week. The ticker is BTC-MOVE-WK-[EXPIRY]. For example, BTC-MOVE-WK-0806 is the weekly BTC MOVE contract expiring at the close of August 6th.  Note that as they’re currently structured, weekly contracts expire on Friday’s daily close.  

Quarterly MOVE contracts expire to the absolute value of the distance BTC has moved from open to close in a roughly-three-month period. The ticker is BTC-MOVE-[YEARQ#].  For example, BTC-MOVE-2021Q3 is the quarterly BTC MOVE contract expiring at the daily close of September 24th (Q3), 2021.  

##How do MOVE contracts work?
Consider a daily MOVE contract such as BTC-MOVE-0806. This contract is available to be traded during the previous day (0805) as a futures contract.  At the end of the proper contract day (0806), it will expire to the absolute value of the difference between BTC’s open and close price for the assigned day.  Because price is determined by the absolute value of the move, this can be considered a non-directional trade.  

##MOVE Expiry Prices
MOVE products expire to the absolute value of the difference between the TWAP price of underlying over the first hour and the TWAP price of the underlying over the last hour of their expiration time, measured in UTC.

So, for example, BTC-MOVE 2018-08-30 expires to ABS[(BTC Index TWAP from 2018-08-30 23:00:00-23:59:59 UTC) - (BTC Index TWAP from 2018-08-30 00:00:00-00:59:59 UTC)].
There will be a new MOVE contract every day to trade the next day's move, in addition to one to trade the current day's move.  There will also be a MOVE contract to trade the current week and the three weeks after it.  Similarly, there will be a new quarterly MOVE contract each quarter, and the three quarters after it will also trade. Every MOVE contract's underlying product is the FTX BTC spot index, and all other references to BTC in this article really mean the BTC index.

##MOVE, Options, & Volatility
MOVE contracts are straddles with a strike price equal to the TWAP of the first hour of their expiration period and underlying expiration price equal to the TWAP of the last hour of their expiration period.

A highly volatile product is expected to undergo moves of tremendous magnitude.  If you assume that products follow a Gaussian distribution, then the expected value of the absolute value of a product's move should be sqrt(2/pi) times the product's daily volatility (or weekly volatility for weekly MOVE contracts).  This means that daily MOVE contracts should be worth roughly 80% of the product's daily volatility.

##Margin & MOVE
Each MOVE contract requires margin based on the price of the underlying index.  This means that a single MOVE contract requires the same amount of margin as a single BTC contract despite the tremendous price difference.

If you select 20x leverage and want to sell one BTC-MOVE contract when BTC-MOVE is trading at $1000 and BTC is trading at $40,000, you will post $2,000 of collateral.  This means that the margin treatment of a MOVE contract depends only on its underlying index's price and not at all on the price of the MOVE contract itself.
This is because the potential variance in a MOVE contract’s price mimics that of the underlying asset (BTC) so the risk profile is similar.  

**Example:** BTC starts the day trading at $10,000 and doesn't move for 20 hours.  At this point the BTC-MOVE contract expiring at the end of that day is likely trading at close to $0 ($50 or so, more likely).  If BTC then increases 3% in the last 4 hours, BTC-MOVE will expire to $300.  The MOVE contract's price changed by about $250 in the last few hours mirroring the price change of BTC.  The risk of holding a single BTC-MOVE contract is roughly equal to the risk of holding a single BTC, so they require the same amount of collateral.

**Note:** If you long MOVE, the amount of margin you must post is capped at the mark price of the MOVE contract.  This means that your required margin is the lesser of the following—the margin you'd need to post based on the index price, or the mark price of the MOVE contract.

##Liquidation
Liquidations for MOVE work the same as liquidations for other contracts, given the margin requirements.  If your total collateral drops below your required maintenance margin, you will begin to get liquidated.

##Fees
The fees charged on MOVE contracts are the same in magnitude as the fees charged on the underlying spot market.  If your fee rate is 0.04% and you buy one BTC-MOVE when BTC-MOVE is trading at $250 and BTC is trading at $10,000, then your fees will be 0.04% * $10,000 = $4. 

##Extrinsic Value & Time Decay
 Time decay is the reduction in the value of an option as the time to the expiration date approaches. An option's time value is how much time plays into the value—or the premium—for the option. The time value declines—or time decay accelerates—as the expiration date gets closer because there's less time for an investor to earn a profit from the option.
This figure, when calculated, will always be negative, as time only moves in one direction. The countdown for time decay begins as soon as the option is initially bought and continues until expiration. 

The extrinsic value of an option factors in the amount of time left before expiration and the rate of time decay leading up to the expiry. If an investor buys a call option with a few months until expiry, the option will have a greater value than an option that expires in a few days. The time value of an option with little time left until expiry is less since there's a lower probability of an investor making money by buying the option. As a result, the option's price—or premium—declines. 

The option with a few months until expiry will have an increased amount of time value and slow time decay since there's a reasonable probability that an option buyer could earn a profit. However, as time passes and the option isn't yet profitable, time decay accelerates, particularly in the last 30 days before expiration. As a result, the option's value declines as the expiry approaches, and more so if it's not yet profitable.

This is all relevant when considering a MOVE trade because the derivative has a premium attached to it.  If the strike price and index price of the underlying asset are both equal, MOVE will not trade at $0—it will trade at the premium.  

**Example:** Suppose the strike price of the daily MOVE contract is $40,000.  Around midday, BTC falls from $42,000 to $40,000—the index price and strike price are equal at this point.  You take a long MOVE position with a size of 1, paying the cost of the premium.  BTC continues to fall from $40,000 to $39,000, bringing the value of your MOVE position to $1,000 plus the premium.  Three hours later, after a period of consolidation, BTC returns to $40,000—our strike price.  The value of your MOVE contract is once again solely the premium, but now it is a smaller dollar value, and your UPNL is in the red.  This is because time decay (or theta decay) has reduced the value of the premium. 
