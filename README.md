![alt=""](Images/module-19-background.jpeg)

# Background
You work at a startup that’s building a new and disruptive application named KryptoJobs2Go (a fictitious application). Your customers can use KryptoJobs2Go to find fintech professionals from a list of candidates, hire them, and then pay them. As the lead developer, you’ve been tasked with integrating the Ethereum blockchain network into the application. The purpose is to enable the customers to instantly pay their hired fintech professionals with cryptocurrency.

## What You're Creating
The completed fintech_finder.py file, which contains the code that’s associated with the web interface of your application. (The included code is compatible with the Streamlit library.) You’ll write all your code for this Challenge in this file.

_Note_ that by using import statements, you’ll integrate the crypto_wallet.py Python script into the code in this file.
A README.md file that includes screenshots to confirm that by assuming the role of a KryptoJobs2Go customer, you successfully created an Ethereum transaction, including the gas estimate, that pays a KryptoJobs2Go candidate for their work.

## Instructions
* The instructions for this Challenge are divided into the following high-level steps:

* Import Ethereum transaction functions into the KryptoJobs2Go application.

* Sign and run a payment transaction.

* Inspect the transaction in Ganache.

## Step 1: Import Ethereum Transaction Functions into the KryptoJobs2Go Application
Import several functions from the crypto_wallet.py file into the fintech_finder.py file. _Note_ that the latter file contains the code for the customer interface of the KryptoJobs2Go application. And, you’ll import the functions to add wallet operations to this application. In this section, you’ll also assume the role of a KryptoJobs2Go customer (that is, you’ll provide your Ethereum wallet and account information to the application).

## Step 2: Sign and Run a Payment Transaction
Write the code to calculate the wage, in ether, of a fintech professional. The code will base this wage on both the professional’s hourly rate and the number of hours that they worked for a customer. Note that candidate_database in fintech_finder.py contains the hourly rates.

You’ll then write the code that uses the calculated wage to send a transaction that pays the professional. This code should allow the KryptoJobs2Go customer to authorize the transaction with their digital signature. To test this application, you’ll use your own Ethereum account information as the customer account information.

## Step 3: Inspect the Transaction in Ganache
In this section, you’ll test the KryptoJobs2Go application with your newly integrated Ethereum wallet. Specifically, you’ll send a test transaction by using the web interface of the application, and then look up the resulting transaction in Ganache.

# Requirements
## Import Ethereum Transaction Functions into the KryptoJobs2Go Application
To receive all points, you must:

* Import the generate_account, get_balance, and send_transaction functions from the crypto_wallet.py file into the fintech_finder.py file.
* Call the generate_account function, and store the account object.
* Call the get_balance function and pass it the Ethereum account.address.

## Sign and Run a Payment Transaction
To receive all points, you must:

* Calculate the transaction’s total wage.
* Call the send_transaction function, and pass it the account, candidate_address, and wage parameters.
* Return the transaction hash from send_transaction, and display it in the web interface of the application.

## Inspect the Transaction in Ganache
To receive all points, you must:

* Send a transaction by using the KryptoJobs2Go application, and then use the returned transaction hash to verify the transaction in Ganache. In the README.md file of your GitHub repository for this Challenge assignment, include a screenshot from Ganache of the transaction details.

* In your README.md file, include two screenshots from Ganache: one of the sender’s address balance and history and another of the recipient's address balance and history.
