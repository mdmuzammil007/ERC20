# MyToken

## Introduction

Welcome to the documentation for **MyToken**, a custom ERC20 token contract implemented in Solidity. This contract provides basic functionalities for managing tokens, including minting, burning, and transferring tokens.

## Overview

**MyToken** is built on top of the ERC20 standard, which ensures compatibility with a wide range of decentralized applications (dApps), wallets, and exchanges. Additionally, it inherits from the `Ownable` contract, allowing for ownership control and access restriction.

### Features

- **Minting**: Only the owner of the contract can mint new tokens. This feature enables the issuance of tokens to designated addresses.
- **Burning**: Token holders can burn their own tokens, reducing the total token supply. This action is irreversible.
- **Transferring**: Token holders can transfer tokens to other addresses, provided they have a sufficient balance.

## Getting Started

To utilize **MyToken** in your project, follow these steps:

1. **Deployment**: Deploy the contract on the Ethereum blockchain.
2. **Ownership**: Upon deployment, the deployer becomes the owner of the contract.
3. **Minting**: The owner can mint new tokens to designated addresses using the `mint` function.
4. **Burning**: Token holders can burn their tokens using the `burn` function.
5. **Transferring**: Tokens can be transferred between addresses using the `transfer` function.

## Usage

### Minting Tokens

```solidity
function mint(address grantBeneficiary, uint256 grant) external onlyOwnerCanMint
```

To mint new tokens, the owner must call the `mint` function, specifying the beneficiary address and the amount to be minted.

### Burning Tokens

```solidity
function burn(uint256 grant) external
```

Token holders can burn their tokens by calling the `burn` function, specifying the amount to be burned.

### Transferring Tokens

```solidity
function transfer(address grantBeneficiary, uint256 grant) public override returns (bool)
```

Token holders can transfer tokens to other addresses using the `transfer` function, specifying the recipient address and the amount to be transferred.

## License

This contract is licensed under the [MIT License](https://opensource.org/licenses/MIT), granting users the freedom to use, modify, and distribute the code.

**Author**:   Mohammed Muzzamil
**Date**: 25 january 2024
