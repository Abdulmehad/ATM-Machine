Overview:
This Java program simulates a basic ATM system with the functionality to create savings and checking accounts, perform deposits, withdrawals, and check account balances.

Classes and Interfaces:
bankaccount (Abstract Class):

Abstract class representing a generic bank account.
Contains attributes like accountno, accountholdername, and balance.
Abstract methods deposit and withdraw to be implemented by subclasses.
savingaccount (Class extending bankaccount):

Represents a savings account.
Inherits from bankaccount and implements the abstract methods.
Has an additional attribute interestrate and overrides the withdraw method.
checkingaccount (Class extending bankaccount):

Represents a checking account.
Inherits from bankaccount and implements the abstract methods.
Has an additional attribute overdraftlimit and overrides the withdraw method.
atmtransaction (Interface):

An interface defining methods for ATM transactions - withdraw, deposit, and checkbalance.
atm (Class implementing atmtransaction):

Represents the ATM system.
Implements methods for account management, withdrawal, deposit, and checking balance.
Maintains an ArrayList of bankaccount objects.
ATMmain (Main Class):

Contains the main method to execute the ATM program.
Creates an instance of the atm class and initializes sample saving and checking accounts.
Provides a user interface for creating accounts and performing transactions.
Usage:
Creating Accounts:

Choose between saving and checking accounts.
Enter account holder's name.
Managing Accounts:

Deposit funds into an account.
Withdraw funds from an account.
Check the account balance.
ATM Operation:

The ATM class provides a text-based menu for users to interact with their accounts.
Error Handling:

The program includes basic error handling for invalid inputs.
Running the Program:
Compile:

Compile the Java program using a Java compiler.
Run:

Run the compiled program.
Follow On-Screen Instructions:

Interact with the program by following the on-screen instructions.
Notes:
The program uses a simple random number generator to assign account numbers.
It includes a basic exception handling mechanism for unexpected input.
Disclaimer:
This program is a simplified simulation for educational purposes and may not represent real-world banking systems. Use it at your own risk.
