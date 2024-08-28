# chooser_option

A Chooser Option is an exotic option that gives the holder the flexibility to choose whether the option will be a call or a put at a predetermined decision date during the life of the option. This flexibility allows the holder to decide based on the market conditions at the decision time, making it valuable in uncertain markets.


Underlying Asset (S): The asset on which the option is based (e.g., a stock, index).
Strike Price (K): The price at which the option can be exercised.
Decision Time (t_decision): The time at which the holder must choose whether the option will be a call or a put. This is a fixed point before the option's maturity.
Maturity (T): The time until the option expires.

Call Option: Gives the holder the right to buy the underlying asset at the strike price.
Put Option: Gives the holder the right to sell the underlying asset at the strike price.



At the decision time t_decision, the holder decides whether the option will be a call or a put, based on the conditions of the market. The payoff at maturity depends on the choice made at the decision time.

Call Option Payoff:
If the holder chooses a call option, the payoff at maturity T is:
Payoff_call = max(S_T - K, 0)
Where:
S_T is the price of the underlying asset at maturity.
K is the strike price.

Put Option Payoff:
If the holder chooses a put option, the payoff at maturity T is:
Payoff_put = max(K - S_T, 0)

Chooser Option Payoff:
The holder chooses the option (call or put) that provides the higher payoff:
Payoff = max(Payoff_call, Payoff_put)
