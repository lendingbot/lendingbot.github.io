---
layout: post
title:  "The Long and the Short of Lending on Poloniex"
date:   2016-06-23 10:18:00
categories: Poloniex Margin Lending Trading Cryptocurrency
---

Lending Bitcoin on Poloniex currently earns 0.02% per day.  Compounded annually that’s over 7%.  That’s a pretty impressive yield for a deflationary and appreciating asset like Bitcoin...but...what gives?  Who are you lending to?  Why are they willing to pay you 7% A.P.Y.?  And why would the mostly anonymous borrower ever pay you back?  This post will address these questions as more, as we dive into the fast and frequent world of lending to margin traders on Poloniex.

### Overview

At its core, lending on Poloniex is peer-to-peer Margin Lending.  When you lend to margin traders on Poloniex, you’re lending to people who are attempting to enhance their trading and investing returns by using their existing Poloniex account balances as collateral to borrow even more cryptocurrency.

In traditional financial markets, margin lending is mostly monopolized by the brokers who create the trading platforms.  In the cryptocurrency space, platforms like Poloniex allow peer-to-peer margin lending, where margin loans don’t originate from the platform owners, but from other users of the platform.

What makes this development exciting, is that we can make money on cryptocurrency exchanges from something other than trading.  Lending to margin traders can be a lower risk (though still not risk free) way to earn a significant return on otherwise idle funds.

### Mechanics

The mechanics of lending on Poloniex are straightforward.  Lenders deposit funds to their Poloniex account in the same way that traders do.  They transfer their balances to a lending sub-account and create loan offers for margin traders using the Poloniex loan order book.

Loan offers for a given currency are organized in the order book based on how favorable they are to the borrower.  Loan offers with lower rates and longer maximum durations get priority over loan offers with higher rates and shorter maximum durations.

When Margin traders execute trades that require them to borrow funds, the Poloniex platform will match the trader with the best available loan offer (the one at the top of the order book).  At this point, a loan is opened.  The loan will stay open until the margin trader closes the trade or the maximum duration of the loan is reached.

When a trade is closed, the interest on the trade is paid from the margin trader to the lender.  The interest is calculated based on the agreed upon rate and the duration of the loan.

### Supply and Demand

In the lending market, demand comes from margin traders who want to borrow a specific cryptocurrency for the purpose of speculation.  Demand from margin traders will cause lending rates to rise as they compete for loans.

Supply in the lending market originates from lenders who wish to earn a return on their idle funds by lending them out.  Excess supply will cause lending rates to fall because they will compete to offer the best rate for margin traders.

Just a few months ago, compound annual lending rates for Bitcoin on Poloniex were as high as 40%.  It may seem unintuitive, but this huge increase in demand for Bitcoin loans was caused by the large increase in the Ether price.

The Ether price increase created lots of demand from margin traders who wanted to borrow Bitcoin.  The traders then sold this Bitcoin for Ethereum with the hopes that the Ether would continue to increase in price.

### Benefits over other forms of Peer to Peer Lending

When you lend on BTCJam or other peer to peer services, the borrower has full custody of the funds they’ve borrowed.  Default rates in this scenario are high, especially in the cryptocurrency space where the lender has little recourse if the borrower defaults.  

When you lend to margin traders on platforms such as Poloniex, it’s impossible for the borrowed funds to leave the platform.  As soon as the borrower closes their trade, the funds are automatically returned to the lender.  Additionally, Poloniex is able to implement strict risk controls for borrowers, where the borrower's loan is auto-liquidated if their available collateral drops below a certain threshold.

As of this writing, our lending bot has issued 108, 000 loans, with 0 defaults.  That’s an unheard of ratio in the peer to peer lending space, and is thanks to the ‘climate controlled’ environment in which these loans are issued.

### Risks

Lending to margin traders on Poloniex carries three main risks for the lender.  

Exchange insolvency:  The cryptocurrency space has been plagued with exchange hacks and failures, such as the now infamous Mt. Gox.  If an exchange becomes insolvent or otherwise loses customer funds, there is a high probability of a substantial or total loss for the lender.
Mitigation: Diversify your lending across multiple exchanges.  Do diligence about the exchange that you’re using.  Frequent exchange outages, and poor infrastructure are red flags.

Exchange outage: Exchange outages, and periods of high volatility are highly correlated, because the increased trading volume caused by the volatility taxes the exchanges servers.  A temporary exchange outage during a period of high volatility could lead to a situation where margin traders lose all of the collateral in their accounts, and then some.  In this situation, the trader would be unable to repay the entirety of their margin loan.

Mitigation: Same as above.

Inability to liquidate:  When your funds are on loan to margin traders, they are not available to you until the margin loan has matured.  A price ‘crash’ on an asset that you are lending, will almost always be in the favor of the borrower.  Because they will be making money from the crashing price, they will be less inclined to close the loan, and you as the lender will be left holding the bag.

Mitigation: Lend currencies that you believe will appreciate in value and are willing to hold for the long-term.

### Conclusion

While it is not without risk, peer to peer margin lending can be an effective way to earn a significant amount of interest on idle cryptocurrency.  It carries significantly less risk than trading, and should carry a substantially lower default rate than peer to peer lending on platforms where users have full custody of their borrowed funds.  Do your diligence, and never invest or lend more than you can afford to lose!



[jekyll-gh]: https://github.com/mojombo/jekyll
[jekyll]:    http://jekyllrb.com
