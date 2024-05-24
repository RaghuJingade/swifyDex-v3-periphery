# SwifyDex V3 Periphery

This repository contains the periphery smart contracts for the SwifyDex V3 Protocol.
For the lower level core contracts, see the [uniswap-v3-core]repository.


```typescript
import {
  abi as SWAP_ROUTER_ABI,
  bytecode as SWAP_ROUTER_BYTECODE,
} from 'swifydex-v3-periphery/artifacts/contracts/SwapRouter.sol/SwapRouter.json'

// deploy the bytecode
```

This will ensure that you are testing against the same bytecode that is deployed to
mainnet and public testnets, and all code will correctly interoperate with
your local deployment.

## Using solidity interfaces

The swifydex v3 periphery interfaces are available for import into solidity smart contracts
via the npm artifact `@swifydex-v3-periphery`, e.g.:

```solidity
import 'swifydex-v3-periphery/contracts/interfaces/ISwapRouter.sol';

contract MyContract {
  ISwapRouter router;

  function doSomethingWithSwapRouter() {
    // router.exactInput(...);
  }
}

```
