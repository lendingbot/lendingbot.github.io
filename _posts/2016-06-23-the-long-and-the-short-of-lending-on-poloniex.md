---
layout: post
title:  "The Long and the Short of Lending on Poloniex"
date:   2016-06-23 10:18:00
categories: Poloniex Margin Lending Trading Cryptocurrency
permalink: /margin-lending-basics
---
Lending Bitcoin on Poloniex currently earns 0.02% per day.  Compounded annually that’s over 7%.  That’s a pretty impressive yield for a deflationary and appreciating asset like Bitcoin...but...what gives?  Who are you lending to?  Why are they willing to pay you 7% A.P.Y.?  And why would the mostly anonymous borrower ever pay you back?  This post will address these questions as more, as we dive into the fast and frequent world of lending to margin traders on Poloniex.

### Overview
At its core, lending on Poloniex is peer-to-peer margin lending.  When you lend to margin traders on Poloniex, you’re lending to people who are attempting to enhance their trading and investing returns by using their existing Poloniex account balances as collateral to borrow even more cryptocurrency.

In traditional financial markets, margin lending is mostly monopolized by the brokers who create the trading platforms.  In the cryptocurrency space, platforms like Poloniex allow peer-to-peer margin lending, where margin loans don’t originate from the platform owners, but from other users of the platform.

What makes this development exciting is that we can make money on cryptocurrency exchanges from something other than trading.  Lending to margin traders can be a lower risk (though still not risk free) way to earn a significant return on otherwise idle funds.

### Mechanics

The mechanics of lending on Poloniex are straightforward.  Lenders deposit funds to their Poloniex account in the same way that traders do.  They transfer their balances to a lending sub-account and create loan offers for margin traders using the Poloniex loan order book.
<hr/>
![A picture of the Poloniex ETH lending order book]({{ site.baseurl }}assets/images/eth-lending-example.png)
<sub>The Poloniex ETH lending order book.  The loan offers with the lowest rates will be filled first.  Placing an offer at 0.045% (that's about 20% APY) will put us first in line.  Our Poloniexlendingbot.com service auotmates this part of the process.</sub>
<hr/>

Loan offers for a given currency are organized in the order book based on how favorable they are to the borrower.  Loan offers with lower rates and longer maximum durations get priority over loan offers with higher rates and shorter maximum durations.

When margin traders execute trades that require them to borrow funds, the Poloniex platform will match the trader with the best available loan offer (the one at the top of the order book).  At this point, a loan is opened.  The loan will stay open until the margin trader closes the trade or the maximum duration of the loan is reached.

When a trade is closed, the interest on the trade is paid from the margin trader to the lender.  The interest is calculated based on the agreed upon rate and the duration of the loan.

<hr/>
![Recently closed loans from the Poloniexlendingbot dashboard]({{ site.baseurl }}assets/images/recently-closed.png)
<sub>An image of recently closed loans from the Poloniexlendingbot.com dashboard.  Lending to margin traders can result in hundreds of micro-loans per day.</sub>
<hr/>

### Supply and Demand

In the lending market, demand originates with margin traders who want to borrow a specific cryptocurrency for the purpose of speculation.  Demand from margin traders will cause lending rates to rise as they compete to borrow funds.

Supply in the lending market originates with lenders who wish to earn a return on their idle funds by lending them out.  Excess supply will cause lending rates to fall because lenders will compete to offer the best rates to the margin traders.

Just a few months ago, compound annual lending rates for Bitcoin on Poloniex were as high as 40%.  It may seem unintuitive, but this huge increase in demand for Bitcoin loans was caused by the large increase in the Ether price.

The Ether price increase created lots of demand from margin traders who wanted to borrow Bitcoin.  The traders then sold this Bitcoin for Ether with the hopes that the Ether would continue to increase in price.

### Benefits over other forms of P2P Lending

When you lend on [BTCJam](https://btcjam.com/) or other peer to peer services, the borrower has full custody of the funds they’ve borrowed.  Default rates in this scenario are high, especially in the cryptocurrency space where the lender has little recourse if the borrower defaults.  

When you lend to margin traders on platforms such as Poloniex, it’s impossible for the borrowed funds to leave the platform.  As soon as the borrower closes their trade, the funds are automatically returned to the lender.  Additionally, Poloniex is able to implement strict risk controls for borrowers, where the borrower's loan is auto-liquidated if their available collateral drops below a certain threshold.

As of this writing, our lending bot has completed 108,000 loans, with 0 defaults.  That’s an unheard of ratio in the peer to peer lending space, and is thanks to the tightly controlled environment in which these loans are issued.

### Risks

Lending to margin traders on Poloniex carries three main risks for the lender.  

<strong>Exchange insolvency:</strong>  The cryptocurrency space has been plagued with exchange hacks and failures, such as the now infamous Mt. Gox.  If an exchange becomes insolvent or otherwise loses customer funds, there is a high probability of a substantial or total loss for the lender.

<strong>Exchange outages:</strong> Exchange outages, and periods of high volatility are highly correlated because the increased trading volume caused by volatility taxes the exchange's servers.  A temporary exchange outage during a period of high volatility could lead to margin traders losing all of the collateral in their accounts as well as some of their borrowed funds.  In this situation, the trader would be unable to repay the entirety of their margin loan.

<strong>Currency Risk:</strong>  When funds are on loan to margin traders, they are not available to be exchanged until the margin loan has matured.  A price ‘crash’ on an asset that you are lending, will frequently be in the favor of the borrower.  Because the borrower will be making money from the crashing price, they will not want to close the loan, and you as the lender could be left holding the bag.

### Conclusion

While it is not without risk, peer to peer margin lending can be an effective way to earn a significant amount of interest on idle cryptocurrency.  It carries significantly less risk than trading, and should carry a substantially lower default rate than peer to peer lending on platforms where users have full custody of their borrowed funds.  Do your diligence, never invest or lend more than you can afford to lose, and consider <a href="https://www.poloniexlendingbot.com">automating your lending</a> for higher returns with less effort!

[jekyll-gh]: https://github.com/mojombo/jekyll
[jekyll]:    http://jekyllrb.com
