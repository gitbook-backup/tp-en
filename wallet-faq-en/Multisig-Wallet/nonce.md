# What is Multisig nonce?

The multisig contracts have a so called nonce. This is to ensure that each transaction can be executed only once so no replay attacks are possible. The multisig nonce is equivalent to the nonce of externally owned accounts (EOAs).

The current multisig nonce can be found in the wallet details of multisig wallet by checking the nonce of your multisig wallet on-chain.

Assuming the current multisig nonce is x, the next transaction to be executed will have to have a multisig nonce of x. In case you change the nonce to something higher, your transaction will have to wait. In case you change it to something lower, it will never be executed successfully. This logic is defined in the multisig smart contract.

The multisig nonce can only be configured when initiating a multisig transaction, i.e. it is not possible to modify it as "second signer" of a transaction.
