# Transaction Pending Forever? Here is How You Make it Successful Faster!

Recently, we have got several pieces of feedback from our users that it takes forever for their transfer to arrive. After consulting the Explorer, it appears that those transactions are still pending after a long while, which is mainly due to a low Gas Price set by the users.

When encountering a similar situation, the user is advised to restart the transaction with a higher Gas Price and make the nounce value equal to the previous transaction, so that the old transaction will be replaced.

### Here is how you do it step by step <a id="4c22"></a>

1. Tap on ETH in TokenPocket and select the pending transaction, copy the receiver’s address.

![1.jpg](https://tokenpockethelpsupport.zendesk.com/hc/article_attachments/900002283123/1.jpg)

Take a quick look into the transaction’s details in one of the Explorers.

![2.jpg](https://tokenpockethelpsupport.zendesk.com/hc/article_attachments/900002283103/2.jpg)

2. Redo the transaction and set a higher Gas Price. \(Here we use ETH as an example due to its low GAS Price.\)

![3.jpg](https://tokenpockethelpsupport.zendesk.com/hc/article_attachments/900002305626/3.jpg)

3. After a while, you will be able to see the successful transaction. In terms of the old pending transaction, you will see a ‘’Dropped & Replaced” in Status and a new transaction hash, which means that the old transaction has been replaced by the new hash.

![4.jpg](https://tokenpockethelpsupport.zendesk.com/hc/article_attachments/900002305646/4.jpg)

The above shows how to redo the transaction, but is it possible to cancel the pending transaction and refund the transfer?

The answer is yes. You will have to start a new transaction to your own address with a reasonable Gas Price. You will see the previous pending transaction canceled after the current one goes successful.

![5.jpg](https://tokenpockethelpsupport.zendesk.com/hc/article_attachments/900002283203/5.jpg)

_Note: TokenPocket now supports Gas Station for Ethereum, so users do not have to worry if they don’t have enough Gas. Later on, we will add a Transaction Acceleration function for users. Please stay tuned!_

###  

### You may want to know <a id="2ab5"></a>

Gas refers to the fee, or pricing value, required to successfully conduct a transaction or execute a contract on the Ethereum blockchain platform. A transaction fee is determined by Gas Limit and Gas Price, which can be demonstrated as follows: Transaction fee = Gas Limit \* Gas Price. Actually, the real amount of transaction fee is lower than this as the Gas Limit is the maximum value. However, if the Gas Limit is set too low, the transaction will be rejected but the Gas won’t be refunded. So users normally set a relatively high Gas Limit.

The unit of Gas Price is Gwei, and 1 ETH equals 1 billion Gwei. Normally, Gas Price is about several Gweis. When you set a high Gas Price for a transaction, miners are likely to process your transaction first, and hence, your transaction will be confirmed quickly.

