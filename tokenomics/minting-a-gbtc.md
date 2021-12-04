# Minting a gBTC

To mint a gBTC, first deposit at a 191 : 1 ratio [Toucan Carbon Token](https://docs.toucan.earth/protocol/bridge/tco2-toucan-carbon-tokens)  & [WBTC](https://wbtc.network) into the [SushiSwap Liquidity Pool](https://github.com/sushiswap/sushiswap/blob/canary/contracts/uniswapv2/UniswapV2Pair.sol) this contract returns a pair liquidity provider token called gBTC LP.&#x20;



gBTC LP represents the token holders pro-rata distribution of the pool. For example, if there are 19,100 TC02 tokens and 100wBTC and the LP token is 0.01 gBTC LP. That user would have permission to mint 100 \* 0.01 = 1 gBTC.&#x20;



Now, that the user has .01 gBTC LP tokens they would then interface with the gBTC mint contract and wrap their gBTC LP token into gBTC according to the formula of WBTC in the liquidity pool multiplied by the users amount of gBTC LP tokens.&#x20;



