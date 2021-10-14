# What are Transaction Tips?

Tips are a transaction fee option. In Polkadot and Kusama network, users are allowed to add tips to a transaction to accelerate its approval by making it a priority for miners.

**Note:**

1.Tips are optional. Users are allowed to choose to pay tips according to their own situation. 

2.Under the same conditions, minors will approve the transactions with tips first. 

## How is the transaction fee calculated in Polkadot and Kusama?

The transaction fee in Polkadot and Kusama network are decided by the following three factors:

**a.Byte length fee**

Byte length fee is the product of the fee per byte and the size of the transaction. 

 **b.Weight fee **

Weight is a fixed number designed to manage the time it takes to verify the block. Each transaction includes basic weight and dispatches weight. The basic weight describes the cost involved in the transaction (such as signature verification), and the dispatch weight describes the time to execute the transaction. The weight fee of a transaction is the product of the total weight of a transaction and the price per weight. 

**c.Tips (optional)**

Tips are a type of optional transaction fee. Users are allowed to pay tips to accelerate the approval of the transaction.

The transaction is composed of the three above-mentioned fees and is deducted from the user’s account before the execution of the transaction. A certain portion of the fee belongs to the block producer and the remaining part goes to the Treasury. In the Genesis of Polkadot, 20% goes to the block producer and 80% goes to the Treasury.
