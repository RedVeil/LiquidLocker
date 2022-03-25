
Booster.sol is our main deposit contract for LP tokens. (also does voting)

BaseRewardPool.sol is used as the main reward contract for all LP pools and cvxCrv.
cvxRewardPool.sol is the staking contract for cvx.
There are not many differences between the two types of contracts except for the cvx contract deposits rewarded CRV into the CrvDepositor and is exchanged to cvxCRV before being claimed.

--CVX apr in pools is simply a function of the allocated crv weights. CVX is minted whenever a user claims CRV.
This means that all LP pools, as well as the cvxCRV rewards pool will mint CVX when claiming CRV rewards from the pool.  Take note that CVX pool does not mint more CVX, as rewards received is cvxCRV and not vanilla CRV.