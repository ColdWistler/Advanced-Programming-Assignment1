Rural Bank Account Management System (RBAMS)
📘 Project Overview

The Rural Bank Account Management System is a console-based Java application developed to simulate basic banking operations for the Rural Bank of Nepal (RBN). It aims to offer simple, secure, and efficient financial services like savings and current accounts tailored to remote and rural populations.
📦 Features

    Support for multiple account types: Savings and Current

    Interest application on savings accounts

    Overdraft support for current accounts

    Secure transactions with custom exception handling

    Object-Oriented Programming principles implemented throughout

🧱 Class Design
1. Abstract Class: BankAccount

    Common attributes: accountHolderName, accountNumber, balance

    Common methods: deposit(), withdraw(), displayDetails()

2. Derived Classes

    SavingsAccount:

        Adds method to apply interest

        Restricts withdrawals beyond balance

    CurrentAccount:

        Supports a predefined overdraft limit

        Allows negative balance up to limit

3. Customer Class

    Aggregates multiple accounts

    Can perform operations across all linked accounts

4. Interface (Optional): Transaction

    May define standard banking operations for implementation flexibility

🔐 Exception Handling

    Custom Exception: InsufficientBalanceException

        Thrown when withdrawal rules are violated

        Caught with meaningful user messages

✅ Supported Operations

    Deposit into any account

    Withdraw from account (rules applied)

    Add interest to savings accounts

    Handle overdraft logic for current accounts

    Display details of all accounts linked to a customer
