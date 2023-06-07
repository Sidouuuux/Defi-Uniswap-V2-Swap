
# ✨ Uniswap V2 Swap ✨
Solidity smart contract that enables users to swap tokens on the Uniswap V2 decentralized exchange. It provides functions for swapping WETH (Wrapped Ether) for DAI in a single hop, as well as swapping DAI for WETH and then WETH for USDC in multiple hops. There are also functions for swapping tokens while ensuring an exact amount of the desired token is received. The contract interfaces with the Uniswap V2 Router and ERC20 token contracts to perform the token swaps.
# Requirements 🔧

- [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
  - You'll know you did it right if you can run `git --version` and you see a response like `git version x.x.x`
- [Foundry](https://book.getfoundry.sh/getting-started/installation)
  - You'll know you've installed Foundry right if you can run:
    - `forge --version` and get an output like: `forge x.x.x`

# Usage 📝

## Deploy 🚀

```
forge create --rpc-url INSERT_RPC_API_ENDPOINT \
--private-key YOUR_PRIVATE_KEY \
src/UniswapV2Swap.sol:UniswapV2Swap
```

### Compile 📝

```
forge build
```

## Testing 🧪

```
forge test --fork-url FORK_URL -vvv
```


## Generate Documentation 📝

You can generate documemtation by adding NatSpecs to your contract and run:

```
forge doc --serve --port 4000
```
## Estimate gas 💸

You can estimate gas running:

```
forge test --fork-url FORK_URL -vvv --gas-report
```