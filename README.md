# ERC20 Token Contract

This is a basic implementation of an ERC20 token in Solidity, which is a standard interface for fungible tokens on the Ethereum blockchain.

## Overview

- **Total Supply**: Tracks the total supply of tokens.
- **Balance Of**: Maps addresses to their respective token balances.
- **Allowance**: Maps addresses to the amount they are allowed to spend on behalf of another address.
- **Name**: Name of the token ("Solidity by Example").
- **Symbol**: Symbol of the token ("SOLBYEX").
- **Decimals**: Number of decimal places used by the token (18).

## Functions

- `transfer(address recipient, uint amount)`: Transfer tokens from the sender's address to the recipient's address.
- `approve(address spender, uint amount)`: Approve another address to spend tokens on your behalf.
- `transferFrom(address sender, address recipient, uint amount)`: Transfer tokens on behalf of the sender.
- `mint(uint amount)`: Mint new tokens and assign them to the sender's address.
- `burn(uint amount)`: Burn a specific amount of tokens from the sender's address.


# Vault Smart Contract

This is a smart contract for a vault that holds a specific ERC20 token. It allows users to deposit and withdraw tokens based on the share of the total supply they own.

## Overview

- **Token**: Address of the ERC20 token this vault is associated with.
- **Total Supply**: Total shares of the vault.
- **Balance Of**: Maps addresses to their respective share balances.

## Functions

- `deposit(uint amount)`: Allows users to deposit tokens into the vault, minting shares for them.
- `withdraw(uint shares)`: Allows users to withdraw tokens from the vault, burning their shares.
