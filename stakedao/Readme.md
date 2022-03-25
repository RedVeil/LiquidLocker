In the StakeDao system user can not vote on emissions of the underlying protocol. Instead they vote on SDT emissions for strategies and the locker. StakeDao can than use the full voting power in the underlying protocol to decide where to allocate its emissions the best.


User deposits in to `Depositor` -> Max locks all token in `FXSLocker` + mints `sdToken` + may deposit into `LiquidityGauge` (stake) to receive sdt emissions and full boost on deposits
`FXSAccumulator` accumulates rewards from maxLocking FXS and distributes them to the `LiquidityGauge`.
-- The only reason not to lock or to unstake is to either provide liquidity on curve or to sell into the underlying token.