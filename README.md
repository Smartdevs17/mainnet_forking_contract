# Contract README

This contract is designed to facilitate the swapping of tokens on the Ethereum blockchain using the Uniswap V2 protocol. It allows users to swap USDC for DAI and vice versa, with the option to add liquidity to the USDC-UNI pool.

## Functions

### `swapTokensForExactTokens`

This function swaps a specified amount of USDC for DAI. It takes the following parameters:

* `amountOut`: The exact amount of DAI to receive.
* `amountInMax`: The maximum amount of USDC to spend.
* `path`: An array of token addresses, specifying the path of the swap (USDC -> DAI).
* `to`: The address to receive the DAI.
* `deadline`: The timestamp by which the transaction must be executed.

### `addLiquidity`

This function adds liquidity to the USDC-UNI pool. It takes the following parameters:

* `tokenA`: The address of the first token (USDC).
* `tokenB`: The address of the second token (UNI).
* `amountADesired`: The amount of USDC to add.
* `amountBDesired`: The amount of UNI to add.
* `amountAMin`: The minimum amount of USDC to add.
* `amountBMin`: The minimum amount of UNI to add.
* `to`: The address to receive the liquidity provider tokens.
* `deadline`: The timestamp by which the transaction must be executed.

## Deployment

To deploy this contract, you will need to have Node.js and Hardhat installed on your system. Follow these steps:

1. Clone the repository.
2. Install the dependencies using `npm install`.
3. Compile the contract using `npx hardhat compile`.
4. Deploy the contract using `npx hardhat run scripts/deploy.ts`.

## Testing

To test the contract, you can use the `npx hardhat test` command. This will run the test suite and report any errors or failures.

## Security

This contract has been designed with security in mind. However, it is essential to perform thorough security audits and testing before deploying the contract to the mainnet.

## Contributing

Contributions are welcome! If you have any suggestions or improvements, please submit a pull request.
