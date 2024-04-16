# Ethereum Contract Deployment Script and Smart Contract

This repository contains a deployment script for an Ethereum smart contract using ethers.js, the smart contract code, and its compiled artifacts.

## Smart Contract: SimpleStorage

The smart contract `SimpleStorage` allows storing and retrieving a favorite number and adding people with their favorite numbers.

### Functions:

- `store(uint256 _favoriteNumber)`: Stores the provided favorite number.
- `retrieve()`: Retrieves the stored favorite number.
- `addPerson(string memory _name, uint256 _favoriteNumber)`: Adds a person with a name and their favorite number.

## Compiled Artifacts

The repository includes compiled artifacts for the `SimpleStorage` smart contract:

- **SimpleStorage_sol_SimpleStorage.abi**: The ABI (Application Binary Interface) file, which contains the contract's interface and function signatures.
- **SimpleStorage_sol_SimpleStorage.bin**: The binary file, which contains the compiled bytecode of the contract.

## Deployment Script

The deployment script interacts with a local Ethereum network (e.g., Ganache or Sepoliatestnet thriugh Alchemy) to deploy the `SimpleStorage` smart contract using the provided ABI and binary files.

## Prerequisites

- Node.js and Yarn installed
- A local Ethereum network running (e.g., Ganache, Sepoliatestnet through Alchemy)
- `.env` file with RPC URL and private key

## Usage

1. Install dependencies:

    ```bash
    yarn install
    ```

2. Update `.env` file with your RPC URL and private key.

3. Run the script:

    ```bash
    node deploy.js
    ```

This README provides an overview of the smart contract, compiled artifacts, deployment script, and usage instructions.
