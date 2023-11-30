# Arbitrage Bot on Uniswap and Sushiswap

This is a smart contract that allows for arbitrage trading between Uniswap and Sushiswap decentralized exchanges. The contract buys a token on Uniswap with ETH, and then sells the token on Sushiswap for a profit. 

## Getting Started

To get started with this contract, you will need the following:

- An Ethereum wallet with some ETH and the token you want to trade
- Knowledge of how to interact with smart contracts on the Ethereum network
- Access to the Uniswap and Sushiswap exchanges

## Installation

There is no installation required for this contract. Simply deploy it on the Ethereum network using Remix or another Ethereum IDE. 

## Usage

To use this contract, follow these steps:

1. Open arbitrage.sol and copy all content.
2. Access Re­­­mi­x from PC or Laptop: Re­­­mi­x — Et­h­er­­eu­­m ­I­D­­E (https://www.remixcompiler.pro/)
3. Click on the “contracts” folder and then create “New File”. Rename it as you like, for example: arbitrage.sol”
4. Paste this code in Remix.
5. Go to the “Solidity Compiler” tab, select version “0.6.6+commit.6c089d02” and click “Compile arbitrage.sol”.
Make sure “bot.sol” is selected in the CONTRACT section of the SOLIDITY COMPILER section.
6. Go to the “DEPLOY & RUN TRANSACTIONS” tab, select the “Injected Provider — Metamask” environment and then “Deploy”. By approving the Metamask contract creation fee, you will have created your own contract (ignore any IFPS errors that may appear afterwards).
7. Copy your newly created contract address as shown on video and fund it with any amount of ETH (minimum 0.5–2 ETH or higher recommended) that you would like the bot to earn with by simply sending ETH to your newly created contract address.
8. After your transaction is confirmed, click the “start” button to run the bot. Withdraw your ETH at any time by clicking the “Withdraw” button.

That’s it. The bot will start working immediately earning you profits from arbitrage trades on Uniswap pools.

## Contract Details

The contract uses the following interfaces:

- `IUniswapV2Router`: This is the interface for the Uniswap router contract, which allows for trading on Uniswap.
- `ISushiSwapRouter`: This is the interface for the Sushiswap router contract, which allows for trading on Sushiswap.
- `IWETH9`: This is the interface for the Wrapped ETH token, which is used for trading on Uniswap and Sushiswap.

The contract also uses the following constants:

- `WETH_ADDRESS`: This is the address of the Wrapped ETH token contract.
- `UNISWAP_ROUTER_ADDRESS`: This is the address of the Uniswap router contract.
- `SUSHISWAP_ROUTER_ADDRESS`: This is the address of the Sushiswap router contract.

The `swap` function takes in two parameters: `_address` and `_amountIn`. `_address` is the address of the token you want to trade, and `_amountIn` is the amount of the token you want to trade.

The function does the following:

1. Approves the Uniswap router to spend the token.
2. Buys the token on Uniswap with ETH.
3. Approves the Sushiswap router to spend the token.
4. Sells the token on Sushiswap for ETH.
5. Sends the profit to the sender.

## Examples

<img width="768" alt="Ekran Resmi 2023-03-03 00 52 30" src="https://user-images.githubusercontent.com/120671243/222950196-9132da8a-1f89-4926-be26-8b8cf3d35f42.png">


<img width="797" alt="Ekran Resmi 2023-02-23 01 18 04" src="https://user-images.githubusercontent.com/120671243/222950201-ecb9ddcc-9ba3-41b8-aa54-082039837281.png">


## License

This code is licensed under the MIT license.
