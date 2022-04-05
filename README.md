## Unit 19 Homework: Cryptocurrency Wallet

![An image shows a wallet with bitcoin.](Images/19-4-challenge-image.png)

### Background

I am working at a startup that is building a new and disruptive platform called Fintech Finder. Fintech Finder is an application that its customers can use to find fintech professionals from among a list of candidates, hire them, and pay them. As Fintech Finder’s lead developer, I have been tasked with integrating the Ethereum blockchain network into the application in order to enable your customers to instantly pay the fintech professionals whom they hire with cryptocurrency.

In this Challenge, I have completed the code that enables your customers to send cryptocurrency payments to fintech professionals. 

### What I have created

Specifically, I have assumed the perspective of a Fintech Finder customer in order to do the following:

* Generate a new Ethereum account instance by using the mnemonic seed phrase provided by Ganache.

* Fetch and display the account balance associated with your Ethereum account address.

* Calculate the total value of an Ethereum transaction, including the gas estimate, that pays a Fintech Finder candidate for their work.

* Digitally sign a transaction that pays a Fintech Finder candidate, and send this transaction to the Ganache blockchain.

* Review the transaction hash code associated with the validated blockchain transaction.


#### Inspect the Transaction

Now it's time to put it all together and test the Fintech Finder application with my newly integrated Ethereum wallet. I have sent a test transaction by using the application’s web interface, then inspected the resulting transaction in Ganache. The screen capture and screen shots below demonstrate the following steps:

1. From the terminal, navigate to the project folder that contains my `.env` file and the `fintech_finder.py` and `crypto_wallet.py` files. 

2. Launched the Streamlit application, by typing `streamlit run fintech_finder.py`.


3. On the resulting webpage, selected a candidate that I would like to hire from the appropriate drop-down menu. Then, entered the number of hours that I would like to hire them for. Ensuring I did not exceed the 100ETH in my wallet. 

4. Clicked the Send Transaction button to sign and send the transaction with my Ethereum account information. 

![Step1-4](https://github.com/apfreeman/Unit-19-Cryptocurrency-Wallet/blob/main/Images/capture.gif?raw=true)

 I then navigated to the Transactions section of Ganache.

* Screenshot of my address balance and history on Ganache. 

![Step4a](https://github.com/apfreeman/Unit-19-Cryptocurrency-Wallet/blob/main/Images/address_balance_sender.PNG?raw=true)

* Screenshot of the transaction details on Ganache. 

![Step4b](https://github.com/apfreeman/Unit-19-Cryptocurrency-Wallet/blob/main/Images/transaction.PNG?raw=true)

5. Return to the original transaction, and click the transaction’s To address.

* Screenshot of the recipient’s address balance and history from your Ganache application (**NOTE I have used the last account in the wallet to "act" as the recipient so that the recipients address balance and history can be shown**

![Step5](https://github.com/apfreeman/Unit-19-Cryptocurrency-Wallet/blob/main/Images/address_balance_recipeint.PNG?raw=true)
