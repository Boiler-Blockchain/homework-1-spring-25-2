# **Homework 1 for BoilerBlockchain's Introduction to Blockchain Course (Spring 2025)**  

## **Setup**  

1. **Download and install Node.js:** [https://nodejs.org/en/download/](https://nodejs.org/en/download/)  
2. **Clone the GitHub repository:**  
```bash
git clone https://github.com/Boiler-Blockchain/homework-1-spring-25-2.git
```
3.	Open a terminal in the cloned folder.
4.	Install dependencies:
```bash
npm install
```

## Introduction

In Homework 1, you will implement a basic bank smart contract in Solidity. The contract allows users to create an account, deposit funds, and withdraw funds while ensuring proper account management.

This assignment introduces Solidity data structures, function design, and contract state modifications.

## Bank Contract Overview

The Bank contract allows users to create a simple account and manage their balance through deposits and withdrawals.

### **The `Account` Struct**  

Each account in the contract consists of:  

- **`owner`**: The Ethereum address of the account holder.  
- **`balance`**: The current balance in the account.  

### **Mappings**  

The contract maintains one mapping:  

- **`accounts`**: Links an Ethereum address to its corresponding `Account` struct.  

---

### **Function Descriptions**  

#### **1. `createAccount` Function (20 points)**  

Allows users to create a new bank account.  

- Ensures that an account is created for the caller.  

#### **2. `deposit` Function (25 points)**  

Enables users to increase their account balance.  

- Accepts a `uint256` amount as a parameter.  
- Adds the amount to the user’s account balance.  

#### **3. `withdraw` Function (25 points)**  

Allows users to reduce their account balance.  

- Accepts a `uint256` amount as a parameter.  
- Subtracts the amount from the user’s account balance.  

## Testing

Testing is an important part of the assignment to ensure that the `AssetFactory` and `MarketPlace` contracts work as expected. The testing suite uses the [Hardhat framework](https://hardhat.org/) to run and manage tests.

### How to Run the Tests
1. Ensure all your smart contract inside the `contracts` folder!

2. Run the test suite on the terminal (make sure you are in the correct directory/file) using:
   ```bash
   npx hardhat test
   ```

This will execute all the test scripts located in the `test` directory.

## Submission (100 points)

Submit the following on Brightspace:

- **Completed Code**: Ensure the code is well-documented and adheres to coding standards.
- **Analysis**: A brief report describing your approach, challenges faced, and learning outcomes.

## Notes

- Make sure to thoroughly test your contracts with the provided test scripts.
- Follow the coding standards discussed in class for smart contract development.
- If you encounter issues, refer to the Solidity documentation or reach out for help during office hours (The schedule can be found in the syllabus on Brightspace)
