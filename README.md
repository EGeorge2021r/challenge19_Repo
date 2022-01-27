# Challenge19_Repo
  Module 19 Challenge

# User Story
- Role: Fintech Finder’s lead developer

- Goal: To develop and test the code that will integrate the Ethereum blockchain network into the application in order to enable your customers to instantly pay the fintech professionals whom they hire with cryptocurrency.

- Reason: Fintech Finder is an application that its customers can use to find fintech professionals from among a list of candidates, hire them, and pay them


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
import streamlit as st
from dataclasses import dataclass
from typing import Any, List
from web3 import Web3
w3 = Web3(Web3.HTTPProvider('HTTP://127.0.0.1:7545'))
import os
import requests
from dotenv import load_dotenv
load_dotenv()
from bip44 import Wallet
from web3 import Account
from web3 import middleware
from web3.gas_strategies.time_based import medium_gas_price_strategy
from crypto_wallet import generate_account
from crypto_wallet import get_balance
from crypto_wallet import send_transaction 

# Explanation and Usage of Streamlit Application
Send a test transaction by using the application’s web interface, and then
look up the resulting transaction hash in Ganache using the following steps:

1. From your terminal navigate to `fintech_finder.py` and `crypto_wallet.py` files.
Be sure to activate your Conda `dev` environment if it is not already active.

2. To launch the Streamlit application, type `streamlit run fintech_finder.py`.

3. On the resulting webpage, select a candidate that you would like to hire
from the appropriate drop-down menu. Then, enter the number of hours that you
would like to hire them for. (Remember, you do not have a lot of ether in
your account, so you cannot hire them for long!)

4. Click the Send Transaction button to sign and send the transaction with
your Ethereum account information. If the transaction is successfully
communicated to Ganache, validated, and added to a block,
a resulting transaction hash code will be written to the Streamlit
application sidebar. See screenshot 1 and 2 below:
![streamlit_web3  interface1](https://user-images.githubusercontent.com/88909565/151270539-8f11db21-68c2-41b7-b87b-31fe4955684c.png)
![Streamlit_web interface 2](https://user-images.githubusercontent.com/88909565/151270575-c814f4c8-f66c-4cec-a346-c32985953fde.png)

5. Navigate to the Ganache accounts tab and locate your account.

6. Navigate to the Ganache transactions tab and locate the transaction. see screenshot below:
![Ganache_Screen shot](https://user-images.githubusercontent.com/88909565/151271007-02421541-cd7d-4414-a75e-827774594ad3.png)
