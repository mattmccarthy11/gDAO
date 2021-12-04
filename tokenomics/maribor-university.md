# Maribor University

**Gnosis Safe**

* Implement gBTC Vault
  * [Deploy Safe Documentation](https://docs.gnosis-safe.io/build/sdks/core-sdk#2.-deploy-a-new-safe)
    * [Gnosis Safe Contracts](https://github.com/gnosis/safe-contracts)
    * @param \_owners List of Safe owners.
      * Professor
      * Matthew
    * @param\_threshold
      * 2 initially then we will change to 3&#x20;

```
import { Safe, SafeFactory, SafeAccountConfig } from '@gnosis.pm/safe-code-sdk'

const safeFactory = await SafeFactory.create({ ethAdapter })

const owners = ['0x<address>', '0x<address>', '0x<address>']
const threshold = 3
const safeAccountConfig: SafeAccountConfig = { owners, threshold }

const safeSdk: Safe = await safeFactory.deploySafe(safeAccountConfig)
```

****

### **Offset.sol: wBTC & BCU deposit contract**&#x20;

****[**Approve Spend of WBTC**](https://docs.openzeppelin.com/contracts/2.x/api/token/erc20#IERC20-approve-address-uint256-)

[**Approve Spend of BCU**](https://docs.openzeppelin.com/contracts/2.x/api/token/erc20#IERC20-approve-address-uint256-)

**Check C02 Offset Ratio of BCU to WBTC**

****[**Transfer from depositor's wallet to Gnosis Safe**](https://docs.openzeppelin.com/contracts/2.x/api/token/erc20#IERC20-transferFrom-address-address-uint256-)

**Calculate Amount of GBTC depositor receives**&#x20;

****[**Mint gBTC equal to Amount** ](https://docs.openzeppelin.com/contracts/2.x/api/token/erc20#ERC20Mintable)

****

****



****

&#x20;
