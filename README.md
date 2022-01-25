# challenge19_Repo



# User Story
Role: Fintech Finder’s lead developer

Goal: To develop and test the code that will integrate the Ethereum blockchain network into the application in order to enable your customers to instantly pay the fintech professionals whom they hire with cryptocurrency.

Reason: Fintech Finder is an application that its customers can use to find fintech professionals from among a list of candidates, hire them, and pay them


# Requirements

- Generate a new Ethereum account instance by using the mnemonic seed phrase provided by Ganache.

- Fetch and display the account balance associated with your Ethereum account address.

- Calculate the total value of an Ethereum transaction, including the gas estimate, that pays a Fintech Finder candidate for their work.

- Digitally sign a transaction that pays a Fintech Finder candidate, and send this transaction to the Ganache blockchain.

- Review the transaction hash code associated with the validated blockchain transaction.

- Once the transaction’s hash code is received, navigate to the Transactions section of Ganache to review the blockchain transaction details.

- To confirm that the transaction have been successfully created, save screenshots to the README.md file in the GitHub repository for this assignment.


# Execution Steps
The execution of this project is broken into three steps:

1. Import Ethereum Transaction Functions into the Fintech Finder Application. This is done by Writing all the codes in the starter code file called fintech_finder.py. The code included in this file is compatible with the Streamlit library.

2. Sign and Execute a Payment Transaction. This is done using the second file called crypto_wallet.py. This file contains the Ethereum transaction functions that was created previously.

3. Inspect the Transaction on Ganache. This is done by integrating these two files to automate the tasks associated with generating a digital wallet, accessing Ethereum account balances, and signing and sending transactions via a personal Ethereum blockchain called Ganache.

# Libraries and dependencies
The following libraries and dependencies were deployed:

Import Ethereum Transaction Functions into the Fintech Finder Application


# Explanation and Usage of Streamlit Application
