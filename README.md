# Java ATM System

## Overview:

This repository contains a Java program that simulates a basic ATM system. The program includes classes for creating savings and checking accounts, performing deposits, withdrawals, and checking account balances. The purpose of this project is to provide a simple example of object-oriented programming in Java.

## Classes and Interfaces:

1. **`bankaccount` (Abstract Class):**
   - Abstract class representing a generic bank account.
   - Contains attributes like `accountno`, `accountholdername`, and `balance`.
   - Abstract methods `deposit` and `withdraw` to be implemented by subclasses.

2. **`savingaccount` (Class extending `bankaccount`):**
   - Represents a savings account.
   - Inherits from `bankaccount` and implements the abstract methods.
   - Has an additional attribute `interestrate` and overrides the `withdraw` method.

3. **`checkingaccount` (Class extending `bankaccount`):**
   - Represents a checking account.
   - Inherits from `bankaccount` and implements the abstract methods.
   - Has an additional attribute `overdraftlimit` and overrides the `withdraw` method.

4. **`atmtransaction` (Interface):**
   - An interface defining methods for ATM transactions - `withdraw`, `deposit`, and `checkbalance`.

5. **`atm` (Class implementing `atmtransaction`):**
   - Represents the ATM system.
   - Implements methods for account management, withdrawal, deposit, and checking balance.
   - Maintains an `ArrayList` of `bankaccount` objects.

6. **`ATMmain` (Main Class):**
   - Contains the `main` method to execute the ATM program.
   - Creates an instance of the `atm` class and initializes sample saving and checking accounts.
   - Provides a user interface for creating accounts and performing transactions.

## Usage:

1. **Creating Accounts:**
   - Choose between saving and checking accounts.
   - Enter account holder's name.

2. **Managing Accounts:**
   - Deposit funds into an account.
   - Withdraw funds from an account.
   - Check the account balance.

3. **ATM Operation:**
   - The ATM class provides a text-based menu for users to interact with their accounts.

4. **Error Handling:**
   - The program includes basic error handling for invalid inputs.

## Running the Program:

1. **Compile:**
   - Compile the Java program using a Java compiler.

2. **Run:**
   - Run the compiled program.

3. **Follow On-Screen Instructions:**
   - Interact with the program by following the on-screen instructions.

## Notes:

- The program uses a simple random number generator to assign account numbers.
- It includes a basic exception handling mechanism for unexpected input.

## Disclaimer:

This program is a simplified simulation for educational purposes and may not represent real-world banking systems. Use it at your own risk.

## License:

This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute the code.
