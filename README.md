# Layer-2 DApp on Blockchain - CS765 Spring 2023 Semester

## Project Overview
This repository contains the implementation of a decentralized application (DApp) for CS765 Spring 2023 Semester. The goal of this project is to create a DApp that facilitates transactions between users based on joint accounts while utilizing blockchain technology. The DApp is implemented using the Solidity programming language and deployed on the Ethereum blockchain.

## Functionalities

### 1. registerUser
Function to register a user and add them to the list of available users for transactions.

### 2. createAcc
Function to create a joint account between two users and track individual contributions to the joint account.

### 3. sendAmount
Function to transfer a whole number amount from one user to another, regardless of joint account status. Transactions are rejected if the user doesn't have sufficient balance.

### 4. closeAccount
Function to terminate a joint account between two users.

## Setup Instructions

1. Follow the instructions provided in the https://docs.google.com/document/d/1IfIwdF6vhf4KYP1OYTwFmgqtdHO6nT7m0JaMH1xCIYo/edit?usp=sharing to set up an Ethereum node on your local machine using Truffle/Ganache.

2. Deploy the smart contract (`DApp.sol`) using Remix or the Ethereum node.

3. Use the provided python script (`client.py`) or your preferred language to interact with the deployed smart contract. The script should be used to register users, create joint accounts, initiate transactions, and close accounts.

## Usage

1. Compile and deploy the smart contract.

2. Run the `client.py` script to simulate interactions with the DApp. The script will register users, create joint accounts, and initiate transactions.

## Results and Analysis

The DApp has been successfully implemented with the following characteristics:
- 100 users registered, forming a connected network.
- Power-law degree distribution observed in the network.
- Combined balance in each joint account follows an exponential distribution with a mean of 10.

After firing 1000 transactions, the success ratio was calculated after every 100 transactions and plotted.

## Conclusion

In this project, we successfully developed a layer-2 DApp on top of the Ethereum blockchain. The DApp enables users to transact through joint accounts, following specified rules for transactions and account management.

For detailed code implementation, refer to the `DApp.sol` smart contract and the `client.py` script.




