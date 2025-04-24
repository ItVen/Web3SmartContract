# Arena Of Faith (AOF) Smart Contracts

This repository contains the smart contracts for the Arena Of Faith (AOF) project, which includes a token contract and a sign-in system.

## Overview

The project consists of two main smart contracts:

1. **AofToken (ACP)**: An ERC20 token contract with permit functionality
2. **SignInSystem (SIS)**: A sign-in system that allows users to sign in with a fee

## Smart Contracts

### AofToken (ACP)

The AofToken is an ERC20 token contract that implements the following features:
- Standard ERC20 functionality
- ERC20Permit extension for gasless approvals
- Initial supply of 1,000,000,000 tokens
- Token name: "Arena Of Faith"
- Token symbol: "ACP"

### SignInSystem (SIS)

The SignInSystem is a contract that manages user sign-ins with the following features:
- Configurable sign-in fee
- Time gap between sign-ins (default: 23 hours)
- Tracking of sign-in statistics
- Owner-only fund management
- Event emission for sign-in activities

## Contract Addresses

- AofToken: [To be deployed]
- SignInSystem: 0x696E0eB647Aa84f6AF662cd92D7A86a0bD0d01bC (opBNB)

## Features

### AofToken Features
- Standard ERC20 token functionality
- Permit functionality for gasless approvals
- Fixed total supply
- Immutable token name and symbol

### SignInSystem Features
- Configurable sign-in fee
- Minimum time gap between sign-ins
- Sign-in statistics tracking
- Fund management capabilities
- Event logging for sign-in activities

## Owner Functions

The SignInSystem contract includes several owner-only functions:
- `fetchFunds`: Withdraw specific amount of funds
- `fetchAllFunds`: Withdraw all contract funds
- `updateRequiredSignGap`: Update the minimum time between sign-ins
- `updateRequiredSignInFee`: Update the required sign-in fee

## User Functions

### SignInSystem
- `signIn`: Sign in with a message and fee
- `getSignerInfo`: Get sign-in statistics for a specific address
- `getSystemInfo`: Get system-wide statistics
- `getContractBalance`: Get the contract's current balance

## Development

### Prerequisites
- Node.js
- Hardhat
- Solidity ^0.8.20

### Installation
```bash
npm install
```

### Compilation
```bash
npx hardhat compile
```

### Testing
```bash
npx hardhat test
```

## License

This project is licensed under the MIT License.
