# Fintech-Finder

A web-based marketplace to find, hire, and pay fintech professional candidates on the blockchain using Ether.

## User Experience
The Fintech Finder app showcases available candidates, including their photo, name, Ethereum account address, FinTech Finder rating, and hourly rate.

   ![FinTech Professional View](https://user-images.githubusercontent.com/69730757/167963576-75f077f7-c2ad-4e75-b1a2-4332dea44caf.png)



The Streamlit UI first displays the available Ether balance in the user's account. Next, the user selects a candidate and inputs the number of hours for which they will be paid. The FinTech Finder displays a preview of the total wage in Ether, along with a Send Transaction button.


   ![Sidebar View](https://user-images.githubusercontent.com/69730757/167962177-7f1dc514-33f4-48ed-b5e4-49a2f41cd338.png)




Upon clicking the Send Transaction button, Fintech Finder calls functions from the Crypto_Wallet file to send the transaction and displays the Validated Transaction Hash.


   ![Validated Transaction Hash](https://user-images.githubusercontent.com/69730757/167962759-3d3852a7-fe73-4b1c-87e1-dae7e179ef13.png)



## Supporting Code

Behind the UI, code in the Fintech Finder 'crypto_wallet' file interacts with a personal Ethereum blockchain called Ganache. Crypto_wallet uses a mnemonic seed phrase to generate new Ethereum accounts. The code calculates the total value of a transaction, including the gas estimate. Crypto_wallet digitally signs and sends transactions to the blockchain, returning a validated hash.

## Result

Upon completion of the transaction, details are stored in the Ganache Transactions block history.

   ![Block History](https://user-images.githubusercontent.com/69730757/167966210-f06906a2-d242-4b46-bb2f-81308a9dbc2e.png)


On the Accounts page, you can see that the user's address (at top) has been debited for multiple transactions and the candidate's address (below) has been credited for the most recent transaction. Wages paid!

   ![Account Balances](https://user-images.githubusercontent.com/69730757/167965005-a9c9e7d5-31c5-45ed-9913-fba9d685e35d.png)

---

## Technologies

The Fintech-Finder app is written in Python 3.10.1 and uses the web3 library.
The web interface is rendered using Streamlit.
Ganache provides the Ethereum blockchain, including transactions and hashing.

---

## Installation Guide

This app can be run in any browser using Streamlit and Ganache.

---

## Contributors

The Fintech-Finder app was written by Kyle Huber in May 2022.

---

# Fintech-Finder
