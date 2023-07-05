# What is Multisig nonce?

Nonce is an important concept in EVM (Ethereum Virtual Machine) multi-signature (multi-sig) transactions, used to ensure that transactions are executed in a specific order. It differs from the Nonce used in regular transactions. In multi-sig transactions, multiple addresses collaborate to perform transactions using a shared multi-signature account for signing and authorization. Each address has its own Nonce value, representing the number of transactions already sent from that address.

The purpose of Nonce is to maintain the order and integrity of transactions, preventing replay attacks and ensuring a consistent execution sequence. It is part of the multi-signature contract and is managed and maintained by the contract. Therefore, the Nonce in multi-sig transactions can exceed the current Nonce value of the sending address.

In multi-sig transactions, maintaining the correct order of Nonces is crucial to ensure transaction consistency and correctness. Multi-sig transactions need to be executed in the correct order based on the Nonce values, ensuring that transactions are executed as expected.

It's important to ensure that the Nonce of a multi-sig transaction aligns with the expected order defined by the multi-signature contract. If the Nonce of a transaction does not match the expected value, the transaction will fail with an error when executed on the chain. Therefore, when sending multiple multi-sig transactions simultaneously, it is necessary to execute the transactions in the correct order by incrementing the Nonce values from small to large. Only when the Nonce of a transaction matches the current expected Nonce value, the transaction can be successfully executed.

In the multi-sig transaction queue, transactions are divided into "current transactions" and "queued transactions". If there are no "current transactions" present, it is necessary to initiate a "current transaction" to ensure that subsequent transactions can be sent out normally. Transactions in the queue must be executed in the correct order, and only after the preceding transactions are confirmed and executed can the subsequent transactions be executed.

By understanding and correctly utilizing the concept of Nonce in multi-sig transactions, we can ensure the order and correctness of transactions, enhancing the reliability and security of multi-signature transactions.

In conclusion, Nonce plays a vital role in EVM multi-signature transactions, ensuring the orderly execution of transactions. By maintaining the correct order of transactions, multi-signature transactions ensure that each transaction is executed as intended, avoiding the issues of transaction duplication or out-of-order execution. This helps to ensure transaction consistency and correctness, enhancing the security and reliability of multi-signature transactions.

<figure><img src="../../.gitbook/assets/英 (1).png" alt=""><figcaption></figcaption></figure>

In the given example, suppose a transaction with a nonce of 2 is required on the blockchain. If a transaction with a nonce of 1 is submitted at that moment, it will fail immediately. Similarly, if a transaction with a nonce of 3 or 4 is submitted, it will also fail instantly. Only by submitting a transaction with a nonce of 2, it can be successful.

As long as the transaction is not broadcasted to the blockchain, it can remain in the transaction queue, awaiting future execution.
