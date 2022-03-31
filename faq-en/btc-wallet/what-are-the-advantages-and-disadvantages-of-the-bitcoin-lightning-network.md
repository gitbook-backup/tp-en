# What are the advantages and disadvantages of the bitcoin lightning network?

Lightning networks can provide significant improvements in scalability, and transaction speeds and transaction rates should be significantly improved without affecting the underlying security of the core protocols. However, there are always two sides to everything. Let's take a look at the advantages and disadvantages of lightning networks.

Advantages of lightning network:

* Fast payments: payments within a given channel can be almost as fast as data being transferred between two nodes over the Internet.
* No trusted third party is required: the two participants in the channel pay each other directly using regular bitcoin transactions, and no third party controls their funds.
* The payment channel can remain open indefinitely: as long as the two parties in the channel continue to work with each other, the channel can remain open indefinitely.
* Across the blockchains: the payment channel can be routed across multiple blockchains if another blockchain supports the same hash function for the hash lock and has the ability to create a time lock.

Disadvantages of lightning network:

The security of lightning network payment may make lightning network not suitable for large payment. The payee needs to sign the recovery transaction before receiving the payment, and a hot wallet is needed to receive the payment, which means there is a risk that the private key will be exposed if a security incident occurs.
