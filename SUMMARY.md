# Table of contents

* [Introduction](README.md)
* [TradFi vs DeFi: Lending](tradfi-vs-defi-lending.md)
* [Market forces x Interest Rate Models](market-forces-x-interest-rates.md)
* [On Indexes](on-indexes/README.md)
  * [Why use indexes?](on-indexes/why-use-indexes.md)
* [Scaling and ATokens](scaling-and-atokens.md)
* [Deposit & Borrow Interest](deposit-and-borrow-interest.md)
* [Stable borrowing](stable-borrowing.md)
* [Liquidation](liquidation/README.md)
  * [oracles](liquidation/oracles.md)

## Primer

* [Bitmap & Masks](primer/bitmap-and-masks/README.md)
  * [padding and bytes](primer/bitmap-and-masks/padding-and-bytes.md)
* [WadRayLibrary](primer/wadraylibrary/README.md)
  * [Math Operations](primer/wadraylibrary/math-operations.md)
  * [Scaling different decimal representations](primer/wadraylibrary/scaling-different-decimal-representations.md)
  * [2's complement](primer/wadraylibrary/2s-complement.md)
* [PercentageMath](primer/percentagemath.md)

## Functions

* [General Execution flow](functions/general-execution-flow.md)
* [Common Functions](functions/common-functions/README.md)
  * [.cache](functions/common-functions/.cache.md)
  * [.updateState](functions/common-functions/.updatestate.md)
  * [.updateInterestRates](functions/common-functions/.updateinterestrates.md)
  * [SupplyCap, BorrowCap](functions/common-functions/supplycap-borrowcap.md)
  * [getFlags](functions/common-functions/getflags.md)
  * [getDecimals](functions/common-functions/getdecimals.md)
  * [calculateUserAccountDataParams](functions/common-functions/calculateuseraccountdataparams.md)
* [supply](functions/supply/README.md)
  * [validateSupply](functions/supply/validatesupply.md)
  * [transfer & mint](functions/supply/transfer-and-mint.md)
  * [isFirstSupply](functions/supply/isfirstsupply/README.md)
    * [isUsingAsCollateralOne, isUsingAsCollateralAny](functions/supply/isfirstsupply/isusingascollateralone-isusingascollateralany.md)
* [withdraw](functions/withdraw/README.md)
  * [get user balance & withdraw amount](functions/withdraw/get-user-balance-and-withdraw-amount.md)
  * [validateWithdraw](functions/withdraw/validatewithdraw.md)
  * [collateral check](functions/withdraw/collateral-check.md)
  * [burn ATokens](functions/withdraw/burn-atokens.md)
  * [Ensure existing loans are not impacted](functions/withdraw/ensure-existing-loans-are-not-impacted.md)
* [borrow](functions/borrow/README.md)
  * [getIsolationModeState](functions/borrow/getisolationmodestate.md)
  * [.validateBorrow](functions/borrow/.validateborrow.md)
  * [Mint debt token](functions/borrow/mint-debt-token.md)
  * [setBorrowing](functions/borrow/setborrowing.md)
  * [update IsolationMode debt](functions/borrow/update-isolationmode-debt.md)
  * [transfer underlying to user](functions/borrow/transfer-underlying-to-user.md)
* [repay](functions/repay/README.md)
  * [get current debt](functions/repay/get-current-debt.md)
  * [validateRepay, paybackAmount](functions/repay/validaterepay-paybackamount.md)
  * [burn debt tokens](functions/repay/burn-debt-tokens.md)
  * [Cleanup + Collect repay](functions/repay/cleanup-+-collect-repay.md)
* [liquidate](functions/liquidate/README.md)
  * [\_calclateDebt](functions/liquidate/\_calclatedebt.md)
  * [validateLiquidationCall](functions/liquidate/validateliquidationcall.md)
  * [getConfigurationData](functions/liquidate/getconfigurationdata.md)
  * [calculateAvailableCollateralToLiquidate](functions/liquidate/calculateavailablecollateraltoliquidate.md)
  * [\_burnDebtTokens](functions/liquidate/\_burndebttokens.md)
  * [liquidate/burn collateral](functions/liquidate/liquidate-burn-collateral.md)
* [swapBorrowRateMode](functions/swapborrowratemode.md)
* [setUserUseReserveAsCollateral](functions/setuserusereserveascollateral.md)

## Contracts

* [AToken](contracts/atoken.md)
* [DefaultReserveInterestRateStrategy](contracts/defaultreserveinterestratestrategy.md)
* [StableDebtToken](contracts/stabledebttoken.md)
* [L2](contracts/l2.md)

## Appendix

* [Simple, Compound, APR, APY](appendix/simple-compound-apr-apy.md)

## Aave Features

* [Risk Management](aave-features/risk-management/README.md)
  * [Supply & Borrow Caps](aave-features/risk-management/supply-and-borrow-caps.md)
  * [Isolation Mode](aave-features/risk-management/isolation-mode.md)
  * [Siloed Borrowing](aave-features/risk-management/siloed-borrowing.md)
* [Other features](aave-features/other-features/README.md)
  * [Repay with ATokens](aave-features/other-features/repay-with-atokens.md)
  * [eMode: High efficiency Mode](aave-features/other-features/emode-high-efficiency-mode.md)
  * [Aave Vault](aave-features/other-features/aave-vault.md)
  * [Portal](aave-features/other-features/portal.md)
