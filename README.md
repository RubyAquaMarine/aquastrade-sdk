# Aquas.Trade SDK

[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
[![npm version](https://img.shields.io/npm/v/@aquastrade/sdk/latest.svg)](https://www.npmjs.com/package/@aquastrade/sdk/v/latest)

In-depth documentation on this SDK is available at [uniswap.org](https://uniswap.org/docs/v2/SDK/getting-started/).

* Uniswap V2 : [v2-sdk](https://github.com/Uniswap/v2-sdk)

* Modify the factory contract address, `init_code_pair_hash` address, ETH address, and chain ID in v2-sdk. Compile and publish to NPM mirror. 

## Running tests

To run the tests, follow these steps. You must have at least node v10 and [yarn](https://yarnpkg.com/) installed.

First clone the repository:

```sh
git clone https://github.com/RubyAquaMarine/aquastrade-sdk.git
```

Move into the uniswap-sdk working directory

```sh
cd aquastrade-sdk/
```

Install dependencies

```sh
yarn install
```

Run tests

```sh
yarn test
```

You should see output like the following:

```sh
yarn run v1.22.4
$ tsdx test
 PASS  test/constants.test.ts
 PASS  test/pair.test.ts
 PASS  test/fraction.test.ts
 PASS  test/miscellaneous.test.ts
 PASS  test/entities.test.ts
 PASS  test/trade.test.ts

Test Suites: 1 skipped, 9 passed, 9 of 10 total
Tests:       3 skipped, 125 passed, 128 total
Snapshots:   0 total
Time:        1.853s
Ran all test suites.
✨  Done in 2.60s.
```

## Skale : gas-is-free

There is no need for native ETH on Skale.network

* Native ETH can be deposited into the SKALE BRIDGE
* SKALE BRIDGE wraps an equivalent and outputs an ERC20 token on the Skale chain : EuropaHub.network
  
## removed from sdk
- swapExactETH
- swapExactTokensForETH

