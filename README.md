# Degen Token Smart Contract 

## Overview

The `EnhancedToken` smart contract is an Ethereum-based ERC-20 token with additional features. It includes functionalities such as minting tokens, burning tokens, transferring tokens, and redeeming virtual appliances. The contract is implemented in Solidity and utilizes the OpenZeppelin library for ERC-20 implementation.

## Features

### ERC-20 Token Standard

The contract complies with the ERC-20 token standard, providing basic functionalities like transfer, mint, and burn.

### Virtual Appliances

The contract introduces the concept of virtual appliances, each with a name, price, and quantity. Users can redeem these virtual appliances by burning a specific amount of tokens.

### User Balances

The contract keeps track of user balances for redeemed virtual appliances. Users can check their balances and withdraw the corresponding tokens.

### Owner Functionality

The contract owner (deployer) has special privileges, including minting tokens, adding appliance quantities, and managing the contract.

## Contract Functions

### `mintTokens`

Owner-only function to mint new tokens and increase the total supply.

### `burnTokens`

Allows users to burn their own tokens, reducing the total supply.

### `transferTokens`

Allows users to transfer tokens to other addresses.

### `redeemAppliance`

Allows users to redeem virtual appliances by burning tokens. Checks for sufficient funds and available appliance quantities.

### `getUserBalance`

Allows users to check their balance of redeemed virtual appliances.

### `withdrawUserBalance`

Allows users to withdraw the corresponding tokens for their redeemed virtual appliances.

### `addApplianceQuantity`

Owner-only function to add quantity to a virtual appliance. Rarely used and intended for contract maintenance.

## Getting Started

1. Deploy the contract on an Ethereum network.
2. Mint initial tokens using the `mintTokens` function.
3. Users can interact with the contract by transferring tokens, burning tokens, and redeeming virtual appliances.
4. The owner can manage the contract, including adding appliance quantities.

## Example Workflow

1. Users mint tokens using the `mintTokens` function.
2. Users transfer tokens to others using the `transferTokens` function.
3. Users burn tokens using the `burnTokens` function.
4. Users redeem virtual appliances using the `redeemAppliance` function.
5. Users check their balances with `getUserBalance` and withdraw tokens with `withdrawUserBalance`.
6. The owner can add quantities to virtual appliances using `addApplianceQuantity`.

## Author

mohammed sahil 

mohammedsahil01421@gmail.com

## License

This smart contract is licensed under the MIT License. See the SPDX-License-Identifier in the contract file for details.
