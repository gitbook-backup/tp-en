# what is UTXO

UTXO is an abbreviation of “Unspent Transaction Output”. Customize UTXO, that is, when you send transactions, you can choose which UTXOs you prefer, use a more economical UTXO combination, or assign a specific UTXO. Moreover, TokenPocket supports lower gas fee settings. With the combination of gas fee setting and custom UTXO, Users can stop worrying about "gas fee insufficient". Users can transfer even the last Satoshi bitcoin. Any Satoshi bitcoin will not waste in the daily transaction or the last transaction.



UTXO: Unspent Transaction Output, is a part of both transaction inputs and outputs in Bitcoin transactions. Each transaction consumes old UTXOs and generates new ones. UTXO-based BTC balances are the sum of the BTC quantities in several UTXOs.

Customizing UTXOs means choosing specific UTXOs when sending a transaction, to use a more economical UTXO combination or specify spending on a specific UTXO for the transaction.

The UTXO model in BTC is very different from the account/balance model in Ethereum or bank cards. Based on UTXO, the BTC balance is the sum of BTC quantities in multiple UTXOs.

For example: A sends 1 BTC to B. C sends 0.5 BTC to B. At this point, B has two UTXOs on their BTC address, and their balance is 1.5 BTC. B's wallet has two UTXOs that can be used: UTXO1: 1 BTC UTXO2: 0.5 BTC

If the account/balance model is used, such as in Ethereum, the balance stored in the account is a summarized ETH balance, which is 1.5 ETH.

UTXOs are like different denominations of paper money in our wallet, such as 5 bills of 100 yuan, 6 bills of 50 yuan, etc. The amount of money in our wallet is just the total amount obtained by adding up the different denominations of paper money.

Once you understand the concept of UTXOs, the process of using UTXOs for transactions becomes easy to understand. When transferring funds, you are paying with UTXOs or combinations of UTXOs. In fact, the process of using UTXOs for transactions is similar to the process of using paper money to pay for purchases.

For example, in the above example, B has two UTXOs on their address, which are 1 BTC and 0.5 BTC. Now, B wants to transfer 0.3 BTC to D. In theory, there are two transfer options for B (ignoring transaction fees for simplicity): Option 1: B uses the 1 BTC UTXO to transfer 0.3 BTC to D and receives 0.7 BTC change. Option 2: B uses the 0.5 BTC UTXO to transfer 0.3 BTC to D and receives 0.2 BTC change.

If B wants to transfer 1.4 BTC to D, they need to spend both UTXOs, and they will receive 0.1 BTC change. (Transaction fees are not considered for the sake of explanation in the above examples).

The amount of transaction fees depends on the wallet type, the number of UTXOs spent, and the number of new UTXOs generated.

TokenPocket's BTC wallet supports custom UTXOs, meaning that when making a transaction, users can choose which UTXO(s) to use, in order to use a more economical UTXO combination or specify spending on a specific UTXO for the transaction, and save on transaction fees.
