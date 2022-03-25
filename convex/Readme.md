
Booster.sol is our main deposit contract for LP tokens. (also does voting)

BaseRewardPool.sol is used as the main reward contract for all LP pools and cvxCrv.
cvxRewardPool.sol is the staking contract for cvx.
There are not many differences between the two types of contracts except for the cvx contract deposits rewarded CRV into the CrvDepositor and is exchanged to cvxCRV before being claimed.