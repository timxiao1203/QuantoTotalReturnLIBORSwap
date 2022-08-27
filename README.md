# Quanto Total Return LIBOR Swap

A quanto total return Libor Swap is a swap where one leg is a regular floating leg paying LIBOR less a constant spread and the other leg makes a single payment at the swap’s maturity equal to a leveraged non-negative return on USD-for-EURO exchange rate paid in CAD. The main focus of the valuation model is the quantoed total return on the FX rate.


The payoff of the leg based on the return of the foreign exchange rate is a payoff of a European call option.  Its present value is given by Black’s formula for futures with the discounting factor equal to the Canadian zero-coupon bond and the future price given.

where 

•	X is the spot USD-for-EURO exchange rate,

•	BU is the price of the US T-maturity zero coupon bond, in general, a bond can be priced like https://finpricing.com/lib/FiBond.html

•	BE is the price of the EURO T-maturity zero coupon bond,

•	 is the correlation between the USD-for-EURO and the USD-for-CAD exchange rates,

•	  is the volatility of the USD-for-EURO exchange rate,

•	  is the volatility of the USD-for-CAD exchange rate,

•	T is the swap’s maturity.

The important point is that the option price depends on the volatilities and correlation of the exchange rates as well as on the interest rates of all the three currencies.

Let XUE(t) be the USD-for-EURO exchange rate at time t, which gives the amount of USD funds exchanged for one EURO. Let XUC(t) be a similar USD-for-CAD exchange rate. Assume further that both rates follow geometric Brownian motions with constant volatilities under the natural probability measure:

Assume the Canadian, US, and EURO short time interest rates rC, rU,  and rE, to be deterministic functions of time.  Then the savings accounts of the respective currencies evolve as follows:

We now form the values of the US and EURO saving accounts converted into the Canadian currency with the Canadian saving account used as a numeraire: 

There must exist a measure under which all the tradeables on the Canadian market, discounted by the Canadian saving account, including CU and CE, are martingales. A standard Brownian motion under this measure w* is coupled with the original Brownian motion:

References:

https://osf.io/p7kn4/download
