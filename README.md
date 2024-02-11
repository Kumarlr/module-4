# BikeToken Smart Contract

This Solidity smart contract, named `BikeToken`, is an ERC20 token implementation tailored for a bike token ecosystem. It includes functionalities for minting, transferring, burning tokens, and redeeming tokens for bike purchases.

## Overview

The `BikeToken` contract provides the following functionalities:

- Token creation with the name "BikeCoin" and symbol "BIKE".
- Minting of tokens by the contract owner.
- Transferring tokens between parties.
- Burning of tokens by token holders.
- Redeeming tokens for bike purchases based on predefined bike prices.

## Usage

To use this contract, deploy it with the required parameters (initial owner address) using any Ethereum development environment or tool. Once deployed, interact with the contract using any Ethereum wallet or through smart contract interactions.

## Contract Functions

### `constructor(address initialOwner)`

Initializes the contract with the specified initial owner address and sets the name and symbol for the token.

### `mintTokens(address beneficiary, uint256 amount)`

Mints `_amount` number of tokens and assigns them to the specified `_beneficiary` address. Only the contract owner can call this function.

### `transferTokens(address recipient, uint256 amount)`

Transfers `_amount` number of tokens from the caller's address to the `_recipient` address.

### `redeemForTokens(uint256 tokenAmount)`

Redeems tokens for a bike purchase based on the provided `_tokenAmount`. The function determines the bike brand to be purchased and burns the corresponding amount of tokens.

### `getBalance()`

Returns the balance of tokens for the caller's address.

### `burnTokens(uint256 amount)`

Burns `_amount` number of tokens from the caller's address.

### `determineBikePurchase(uint256 tokenAmount)`

Determines the bike brand to be purchased based on the provided `_tokenAmount`.

### `getRecentlyPurchasedBike()`

Returns the recently purchased bike brand.

## Author

Chethan Kumar L J

## License

This contract is licensed under the MIT License.
