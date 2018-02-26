This paper has outlined the main design and market mechanism for the dual-class token structure. Further studies can be done in below aspects.

Base Rate Discovery

Arbitrary rate can be used for Class A coupon and it will be traded on premiumn or at discount based on the market required rate of return. However, it is desirable that Class A trades close to its net value, which means the coupon rate for Class A should be chosen close to the market rate. Currently there are few observable proxies in the market. Several centralized exchanges allowing margin trading are charging USD borrow rates in the range of 20% to 40% per annum.

As discussed in section 3.1, the market premium or discount of Class A token may imply USD's borrow rate in this market. As the structure gain attractions, its implied rate could serve as an indication for other USD borrow practice in crypto market.

Optimal Class Ratio and Reset Threshold

It is important to keep leverage for Class B within certain range: not too high so as to protect Class A holders from sudden price drop and not too low so as to keep Class B attractive to leveraged investors. However, it is undesirable that resets, especially downward resets, happen too frequent.

There are two main parameters to be determined, the ratio between Class A and Class B shares, alpha; and the lower limit of Class B net value, h, that triggers downward resets. The Chinese market over the years has concluded a broadly accepted set of parameters: alpha is set to 1, meaning the quantities of Class A versus Class B is 1:1; h being 0.25, meaning a downward reset will be triggered if the underlying price dropped approximately 37% from last reset. This setup has been tested in extreme market events such as the mid-2015 market crash and the early-2016 circuit breaker turmoil, where the reset clauses were all successfully implemented and protected the interests of Class A holders.

We observed that cryptocurrencies have considerably higher volatility than stock market indices. A series of backtestings and Monte Carlo simulations will be performed to investigate the optimal parameters for dual class token structures.

Smoothened Net Value for Class A Token

The net value of Class A token is similar to the dirty value of a bond instrument: the value accumulates over time and drop to par upon resets. The flexibility of smart contract allow more sophisticated coupon settlement than traditional bond market, where the token's net value can be smoothened in between transactions. The detailed implementaiton is beyond the scope of this paper.

Other Coin Underlyings

While the structure discussed in this paper is independent to the underlying cryptocurrency, the liquidity and popularity of the underlying does impact the viability of the structure as market arbitrage is important to ensure the structure trades as designed. In this paper, ETH is used as example, but other popular ERC20 coins such as EOS, ADA can also be considered.