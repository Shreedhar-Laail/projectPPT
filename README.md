# Bank Account Management System

This is a Python program that simulates a basic bank account management system. The program allows users to create different types of accounts (Savings or Current), perform various banking operations such as deposit, withdrawal, balance inquiry, fund transfer, and more.

## Table of Contents

- [BankAccount Class](#bankaccount-class)
- [SavingsAccount Class](#savingsaccount-class)
- [CurrentAccount Class](#currentaccount-class)
- [Main Function](#main-function)
- [Usage](#usage)
- [Author](#author)

## BankAccount Class

The `BankAccount` class is the base class for all types of bank accounts. It contains the following methods:

### __init__(self, account_number, account_holder)

- Constructor to initialize a `BankAccount` instance.
- Parameters:
  - `account_number`: Account number for the new account.
  - `account_holder`: Account holder's name for the new account.

### deposit(self, amount)

- Method to deposit funds into the account.
- Parameters:
  - `amount`: Amount to be deposited.
- Returns:
  - `True` if the deposit is successful, `False` otherwise.

### withdraw(self, amount)

- Method to withdraw funds from the account.
- Parameters:
  - `amount`: Amount to be withdrawn.
- Returns:
  - `True` if the withdrawal is successful, `False` otherwise.

### get_balance(self)

- Method to retrieve the current balance of the account.
- Returns:
  - Current account balance.

## SavingsAccount Class

The `SavingsAccount` class inherits from the `BankAccount` class and includes additional methods specific to savings accounts.

### __init__(self, account_number, account_holder)

- Constructor to initialize a `SavingsAccount` instance.
- Inherits from the `BankAccount` class.

### apply_interest(self)

- Method to apply interest to the account balance.

## CurrentAccount Class

The `CurrentAccount` class inherits from the `BankAccount` class and includes additional methods specific to current accounts.

### __init__(self, account_number, account_holder)

- Constructor to initialize a `CurrentAccount` instance.
- Inherits from the `BankAccount` class.

### overdraft_protection(self)

- Method to apply overdraft protection if the balance is within the overdraft limit.

## Main Function

The program's main functionality is contained within the `main()` function. It provides a menu-based interface for users to perform various banking operations. The available options include creating accounts, depositing money, withdrawing money, checking account balances, transferring funds, and more.

## Usage

1. Run the program by executing the script.
2. Follow the on-screen instructions to select the desired operation from the menu.
3. For account creation, provide the account number, account holder's name, and account type (Savings or Current).
4. For deposit and withdrawal, provide the account number and the transaction amount.
5. For fund transfer, provide the sender's and recipient's account numbers along with the transfer amount.
6. For balance inquiry, provide the account number.

## Author

This program was developed by Shreedhar Kumar Kushwaha.

Feel free to modify and extend this code to meet your specific requirements or add more features to the bank account management system.
