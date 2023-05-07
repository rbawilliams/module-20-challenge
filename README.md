# Joint Savings Account Smart Contract

![alt=""](20-5-challenge-image.png)

This repository contains the Solidity smart contract implementation for a joint savings account. The contract allows two user addresses to control a joint savings account and provides features for depositing and withdrawing funds.

## Background

A fintech startup company aimed to disrupt the finance industry by leveraging their own cross-border, Ethereum-compatible blockchain that connects financial institutions. As part of their efforts to automate financial processes, the team decided to build smart contracts for joint savings accounts. These smart contracts would enable users to create joint savings accounts and perform transactions using Ethereum.

## What You'll Find in This Repository

- joint_savings.sol: This Solidity file contains the implementation of the JointSavings smart contract. It includes variables to store account addresses, withdrawal history, and the contract balance. It also defines functions for depositing, withdrawing, and setting the authorized accounts.

- Execution_Results folder: This folder contains eight images demonstrating the successful execution of the contract's functionality in the Remix IDE's JavaScript VM. The images showcase deposit and withdrawal transactions, as well as the retrieval of relevant information from the smart contract.

## Usage Instructions
To use the JointSavings smart contract and interact with it, follow the steps below:

### Step 1: Create a Joint Savings Account Contract in Solidity
Open the Solidity file named joint_savings.sol in the Remix IDE.

Review the provided starter code and understand the contract structure and variables.

Implement the necessary functions as described in the instructions:

withdraw(uint amount, address payable recipient): This function allows the authorized accounts (accountOne and accountTwo) to withdraw funds from the joint savings account. It checks the recipient's address, ensures sufficient funds, updates the withdrawal history, and adjusts the contract balance accordingly.

deposit() payable: This function enables users to deposit funds into the joint savings account. It updates the contract balance with the deposited amount.

setAccounts(address payable account1, address payable account2): This function sets the authorized accounts for the joint savings account.

Fallback function: This function allows the contract to store Ether sent from outside the deposit function.

### Step 2: Compile and Deploy Your Contract in the JavaScript VM
Compile the smart contract in the Remix IDE.

Ensure that the JavaScript VM is selected as the environment in the "Deploy & Run Transactions" pane.

Click the Deploy button to deploy your smart contract and verify that it deploys successfully.

### Step 3: Interact with Your Deployed Smart Contract
Use the setAccounts function to define the authorized Ethereum addresses that can withdraw funds from the joint savings account.

Example addresses:
Dummy account1 address: 0x0c0669Cd5e60a6F4b8ce437E4a4A007093D368Cb
Dummy account2 address: 0x7A1f3dFAa0a4a19844B606CD6e91d693083B12c0
Test the deposit functionality of the smart contract by sending different amounts of Ether:

Transaction 1: Send 1 Ether as wei.
Transaction 2: Send 10 Ether as wei.
Transaction 3: Send 5 Ether.
After each transaction, use the contractBalance function to verify that the funds were added to the joint savings account.

Test the withdrawal functionality of the smart contract:

Withdraw 5 Ether into accountOne.
Withdraw 10 Ether into accountTwo.
After each withdrawal, use the contractBalance, lastToWithdraw, and ` lastWithdrawAmount` functions to verify that the funds were successfully withdrawn and that the address and amount are correct.

## Execution Results

The Execution_Results folder in this repository contains screenshots capturing the successful execution of the smart contract's functionality in the Remix IDE's JavaScript VM. The screenshots include:

Screenshots of the contract deployment confirmation.

Screenshot of the successful execution of the setAccounts function, setting the authorized accounts for the joint savings account.

Screenshots of the successful execution of the deposit transactions, showing the updated contract balance after each deposit.

Screenshots of the successful execution of the withdrawal transactions, demonstrating the updated contract balance, lastToWithdraw, and lastWithdrawAmount after each withdrawal.

Please refer to the images in the Execution_Results folder for a detailed visual representation of the contract's functionality.

## Conclusion
This repository provides a Solidity smart contract implementation for a joint savings account. The contract allows users to create joint savings accounts, deposit funds, and withdraw funds according to the specified requirements. The provided screenshots in the Execution_Results folder demonstrate the successful execution of the contract's functionality using the Remix IDE's JavaScript VM.

Feel free to explore the code, execute it in the Remix IDE, and refer to the execution screenshots to gain a comprehensive understanding of the smart contract's behavior.

