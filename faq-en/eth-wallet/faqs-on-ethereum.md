# FAQs on Ethereum

**1. Where can I see the ETH transfer records?**

In the case of the TokenPocket wallet, you simply click on your ETH asset to view the transfer history.

**2. How to transfer to the wallet other tokens based on ETH?**

The TokenPocket wallet already supports the ETH and ERC20 protocol, and tokens based on the ETH can be stored or used in the TP wallet. You can transfer to the ETH address.

**3. Can the ETH address created from TokenPocket be transferred to another wallet?**

Of course. All you need to do is export your ETH address private key from the TP wallet and import the private key to another wallet to generate your ETH wallet.

**4. Do you have to worry about CPU issues when playing ETH dapps?**

Unlike ETH transfers, which require fees, EOS transfers are almost "free". Users only need to mortgage a small portion of their EOS to the system, which allocates resources and then enjoys a "free" transfer service. However, the EIDOS mining project appeared in EOS last month, which strained the CPU resources of the whole network and seriously affected the experience of EOS dapps.

The ETH network is a different economic model. In the ETH development smart contract, the cost depend on how you store data on the blockchain to consume gas. Although there is a cost to pay, but you do not consider the problem of resource explosion.

**5. What are the ETH transfer fee and gas?**

Gas, gasoline, is a kind of fuel. ETH transfer fees are calculated based on gas consumption (ETH miner fee = Gas Limit \* Gas Price). Like BTC, ETH transfers also pay for blockchain miners.

ETH transfers are said to consume gas. This value is determined by Gas Price (unit Price) and consumed Gas Limit (quantity). The amount of Gas Limit is generally determined by the ETH smart contract content. Therefore, the higher the Gas Price set by the initiator, the faster the transaction can be packaged. However, ETH can be returned if it has more Gas than it needs.

**6. How to transfer/receive ETH from others?**

Take TokenPocket wallet as an example, click "transfer", enter the transfer address of others, enter the amount and password; On the contrary, click "receive" and send receiving address to others. (note that if the ETH is transferred to the contract account or the address of the exchange, you need to fill in the Memo. ETH transfer needs to consume a small amount of miner fee, namely gas fee)

**7. How does ETH in the wallet sell for cash?**

For sale for cash, we need to withdraw ETH to the exchange and sell them through legal currency trading. However, there is a more convenient way for the TokenPocket wallet to convert ETH into EOS through the swap function of the TP wallet, and then sell EOS through CoinMyDex.

(1)Open ETH wallet, click swap, select EOS, enter the amount of exchange, enter EOS address, and click to start the exchange (swap function has a small amount of handling fee).

(2) After the exchange for EOS, open the CoinMyDex（Currently, this function only supports Chinese users）, choose to trade EOS to sell (the first time to use CoinMyDex needs to click on my account to improve the information).

**8. How to transfer ETH（in the exchange）to wallet?**

Take Huobi to TP wallet for example:

(1)Click "Receive", copy the address or QR code

(2)Open my assets in Huobi, click to withdraw, select the ETH, paste the address or scan the QR code, enter the amount of withdrawing, click to withdraw (note that there will be a handling fee and the minimum amount of withdrawing)

**9. How to purchase ETH assets?**

You can buy it from digital currency exchange such as Huobi.

(1)Register/log in the Huobi account and click trade.

(2) click Fiat, choose to buy, choose ETH, click buy (you can click on the filter, choose the right for your payment method and transaction limit)

(3) click buy, there will be the order information, according to the requirements of payment, click I have paid successfully, the seller will send ETH after checking the funds.

**10. How to retrieve the previous ETH wallet?**

First of all, you should save the mnemonic or private key you created before. If you forget it, you can't get it back.

Enter the previous private key or mnemonic, set the password and the name of the wallet, click to import the wallet can restore the previous wallet.

**11. How to create ETH wallet?**

There are many ways to create an ETH wallet. One of the easiest and most practical ways to create an ETH wallet is to download a TokenPocket.

Selects Ethereum

Create Wallet

Set a wallet name, set the password, click create wallet

Create a wallet will first generate a series of mnemonic, be sure to backup the mnemonic, and then enter the mnemonic in order.

We must backup mnemonic, if you lose your wallet, you can find it by mnemonic.

**12. Transaction Pending Forever? Here is How You Make it Successful Faster!**

Recently, we have got several pieces of feedback from our users that it takes forever for their transfer to arrive. After consulting the Explorer, it appears that those transactions are still pending after a long while, which is mainly due to a low Gas Price set by the users.

When encountering a similar situation, the user is advised to restart the transaction with a higher Gas Price and make the nounce value equal to the previous transaction, so that the old transaction will be replaced.

Here is how you do it step by step

Tap on ETH in TokenPocket and select the pending transaction, copy the receiver’s address.

Take a quick look into the transaction’s details in one of the Explorers.

2\. Redo the transaction and set a higher Gas Price. (Here we use ETH as an example due to its low GAS Price.)

3\. After a while, you will be able to see the successful transaction. In terms of the old pending transaction, you will see a ‘’Dropped & Replaced” in Status and a new transaction hash, which means that the old transaction has been replaced by the new hash.

The above shows how to redo the transaction, but is it possible to cancel the pending transaction and refund the transfer?

The answer is yes. You will have to start a new transaction to your own address with a reasonable Gas Price. You will see the previous pending transaction canceled after the current one goes successful.

Note: TokenPocket now supports Gas Station for Ethereum, so users do not have to worry if they don’t have enough Gas. Later on, we will add a Transaction Acceleration function for users. Please stay tuned!

You may want to know

Gas refers to the fee, or pricing value, required to successfully conduct a transaction or execute a contract on the Ethereum blockchain platform. A transaction fee is determined by Gas Limit and Gas Price, which can be demonstrated as follows: Transaction fee = Gas Limit \* Gas Price. Actually, the real amount of transaction fee is lower than this as the Gas Limit is the maximum value. However, if the Gas Limit is set too low, the transaction will be rejected but the Gas won’t be refunded. So users normally set a relatively high Gas Limit.

The unit of Gas Price is Gwei, and 1 ETH equals 1 billion Gwei. Normally, Gas Price is about several Gweis. When you set a high Gas Price for a transaction, miners are likely to process your transaction first, and hence, your transaction will be confirmed quickly.
