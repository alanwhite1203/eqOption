# Stock Option Product and Valuation

Equity options, which are the most common type of equity derivatives, give an investor the right but not the obligation to buy a call or sell a put at a set strike price prior to the contract’s expiry date. Equity options are derivatives that means their value is derived from the value of an underlying equity. Investors and traders can use equity options to take a long or short position in a stock without actually buying or shorting the stock. This is advantageous because taking a position with options allows the investor/trader more leverage in that the amount of capital needed is much less than a similar outright long or short position on margin. Investors/traders can therefore profit more from a price movement in the underlying stock.

Equity options or stock options provide investors a way to hedge risk or speculate.  Also option trading can limit an investor’s risk and leverage investing potential. Option investors have a number of strategies they can utilize, depending on risk tolerance and expected return. 
Buying call options allows you to benefit from an upward price movement (by either selling the option at a profit or buying the stock at a discount relative to its current market value) while limiting losses to the premium paid if the price declines or remains constant. The right to buy stock at a fixed price becomes more valuable as the price of the underlying stock increases. An option seller earns the premium if the underlying stock price would not change much.
Put options may provide a more attractive method than shorting stock for profiting on stock price declines, in that, with purchased puts, you have a known and predetermined risk. The most you can lose is the cost of the option. If you short stock, the potential loss, in the event of a price upturn, is unlimited. If you have an established profitable long stock position, you can buy puts to protect this position against short-term stock price declines. 
You can limit the risk of stock ownership by simultaneously buying a put on that stock, a hedging strategy commonly referred to as a “married put.” This strategy establishes a minimum selling price for the stock during the life of the put and limits your loss to the cost of the put plus the difference, if any, between the purchase price of the stock and the strike price of the put, no matter how far the stock price declines. This strategy will yield a profit if the stock appreciation is greater than the cost of the put option.




	Equity Option Introduction
	Equity options, which are the most common type of equity derivatives, give an investor the right but not the obligation to buy a call or sell a put at a set strike price prior to the contract’s expiry date. 
	Equity options are derivatives that means their value is derived from the value of an underlying equity. 
	Investors and traders can use equity options to take a long or short position in a stock without actually buying or shorting the stock. 
	This is advantageous because taking a position with options allows the investor/trader more leverage in that the amount of capital needed is much less than a similar outright long or short position on margin. 
	Investors/traders can therefore profit more from a price movement in the underlying stock.

	The Use of Equity Option
	Equity options or stock options provide investors a way to hedge risk or speculate.  Also option trading can limit an investor’s risk and leverage investing potential. 
	Option investors have a number of strategies they can utilize, depending on risk tolerance and expected return.
	Buying call options allows you to benefit from an upward price movement. The right to buy stock at a fixed price becomes more valuable as the price of the underlying stock increases.
	Put options may provide a more attractive method than shorting stock for profiting on stock price declines.
	If you have an established profitable long stock position, you can buy puts to protect this position against short-term stock price declines. 
	An option seller earns the premium if the underlying stock price would not change much.

	Equity Option Payoffs
	The payoff of a call option
Payoff=N*max(S-K,0)
where N – the notional; S – the stock price; K – the strike.
	The payoff diagram of a call option



 

	The payoff of a put option
Payoff=N*max(K-S,0)
where N – the notional; S – the stock price; K – the strike;
	Payoff diagram

 



	Valuation
The present value of call option is given by

 PV(t)=N[S_T Φ(d_1 )-KΦ(d_2)] D_T   
	d_1,2=[ln(S_T⁄K)±(σ^2 T)⁄2]⁄(σ√T)                                                                       
where
  -  the cumulative standard normal distribution function
t   –  the valuation date
T – the maturity date
K – the strike
S_T=[S-PV(D)] e^(r_T (T-t) )  – the equity forward price at T
	PV(D)=∑_(t<τ<T)▒〖d_τ e^(-r_τ (τ-t) ) 〗   - the present value of all dividends between t and T
	d_τ – the discrete dividend paid at τ where t ≤ τ ≤ T
S  - the equity spot price at t
N – the notational principal amount
	D_T=D(t,T)  –  the discount factor from T to t

The present value of a put option is given by

PV(t)=N[KΦ(-d_2 )-S_T Φ(〖-d〗_1 )] D_T   
where all notations are the same as above

The put-call parity
The put-call parity defines a relationship between the price of a European call option and European put option with the identical strike and expiry
C – P = S – D*K
where C – the present value of a call option; P – the present value of a put option; S –the spot stock price; K – the strike; D – the discount factor.


Practical notes
	Equity options are valued via the Black model in the market.
	First, you need to construct an interest zero rate curve by bootstring some most liquity interest rate instruments.
	Second, you need to construct an arbitrage-free volatility surface. <> is using SVI model to construct equity volatility surface. <See the volatility contruction tools here>
	Then you need to calculate equity forward price correctly by taking all dividends into account.
	Finally, you can get the price using the Black formula.

A real world example



Underlying equity	.CSEARC5E
Currency	USD
Strike	150.4292
Maturity Date	2/24/2022
Call or Put	Call
Exercise Type	European
Settlement Type	Physical
Position	598.2881


References:
	
https://finpricing.com/lib/EqWarrant.html
	
https://bitbucket.org/cmrm11/eqoption/downloads/EqOption-6.pdf
	

