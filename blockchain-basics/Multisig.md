# What is a multi-sig wallet?

Corresponding to the multi-signature wallet is the single-signature wallet. If we want to conduct a transfer operation on the blockchain, we need to generate a signature with the wallet. We sign and send the transaction out. This is the way for a typical single-signature wallet and it is also for our usual wallet.

A multi-signature wallet, as the name suggests, is a wallet that requires multiple people to sign to perform an operation. Transferring with a multi-signature wallet often requires >= 1 person to sign and send the transaction before the operation can be completed. When using a multi-signature wallet, we can specify the signature mode of M/N, that is, only M signatures among N persons can complete the operation. For example, the 2/3 signature mode means that two of the three people can sign.

The multi-signature of ETH/ERC20 (including EVM chains such as BSC/BEP20) adopts a lightweight smart contract method.

#### Applicable scenes:

1、When managing assets by multiple people to avoid assets being misappropriated by individuals;

2、Multiple encryptions of assets through multi-signature to enhance asset security;

3、Other security application scenarios.
