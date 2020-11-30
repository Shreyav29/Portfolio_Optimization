# Asset Allocation using Convex Portfolio Optimization

Here we study and compare the asset allocation methodology followed through mean variance portfolio optimization(MVO) and Sharpe Ratio optimization.

```math
SE = $\frac{\sigma}{\sqrt{n}}$
```

## Mean Variance portfolio Optimization 
- In Mean variance optimization, we weigh the risk of the portfolio against the expected return and try to maximise the return while minimizing the varince. 
- MVO allows investors to find the biggest reward at a given level of risk or the least risk at a given level of return.

The objective function is : 
$\max _{w} w^{T} \mu -\frac{\delta}{2} w^{T} \Sigma w$

Subject to Constraints : 

Budget constraint : Portfolio weights should add upto one :  $\sum_{i=1}^{n} w_{i} = 1$

No Short selling : $ w_{i} > = 0 $

The portfolio return should be positive : $w^{T} \mu > 0 $

For the given problem the risk averseness of investor is taken as 1. 


### Analysis : 
- We can see that the mean variance optimization suggests that we invest all our money in the asset D. This might give a superior return right now but it also has high volatility. 
- Due to the high vlatility if the return chnages next period we are bound to rebalance the portfolio. Hence a much better and balanced approach would be to optimize the sharpe ratio. 


## Sharpe ratio Optimization : 

Objective function: 
$$   max \frac{w^{T}r_{p} - r_{f} }{\sqrt{w^{T} \Sigma w}}$$

Subject to Constraints : 

Budget constraint : Portfolio weights should add upto one :  $\sum_{i=1}^{n} w_{i} = 1$

No Short selling : $ w_{i} > = 0 $

The portfolio return should be positive : $w^{T} \mu > 0 $


### Analysis : 
- Although the return of sharpe ratio optimization is less, the volatility has significantly reduced. This suggests that the Sharpe ratio optimiation gives a better result that mean variance optimization. 

