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
