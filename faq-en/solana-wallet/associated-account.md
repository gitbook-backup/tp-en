# Associated account of Solana

In Solana Network, if you need to transfer SPLs, the transfer account and the receiving account should be the associated account, not the wallet account. You only need to enter your wallet account when transferring or receiving, the wallet will search the associated account automatically. If you don’t have the associated account, it will create an associated account for receiving account and it will cost 0.02 SOL. Please make sure that the wallet has enough SOL.

\*SPLs is the derivative coin of Solana.

**What’s the associated account?**

“Associated account” is an important part of the underlying logic of the Solana public chain. Every SPL transfer/receipt needs to be carried out through the associated account of the corresponding token on the chain. The associated account of each wallet address is controlled by the private key and mnemonic.

**How to create an associated account?**

In the process of SPL transfer/receipt, enter the wallet address first and the network will create the associated account automatically, and it will cost 0.02 SOL. The transfer will be finished with this associated account later.

After creation, we only need to enter the wallet account in the process of SPL transfer/receipt, the wallet will automatically find the associated account of the Token, and finish the corresponding transfer/receipt.

**Existing associated account:** To transfer/receipt, enter the wallet account/associated account;

**No associated account:** To transfer/receipt, enter the wallet account, and the network will create an associated account. Creating an associated account requires a handling fee of 0.02 SOL. Please reserve sufficient SOL.

**How to check the associated account?**

1. Enter the Solana Explorer

[https://solscan.io/](https://solscan.io/)

[http://solanabeach.io/](http://solanabeach.io/)

[http://explorer.solana.com/](http://explorer.solana.com/)

2. Enter your wallet address and click \[SPL Token TXs\], 「DESTINATION」will show the associated account of the transfer.

![](../../.gitbook/assets/image%20%2839%29.png)

**ATTENTION:** "Associated account" is only required for SPL transfer/receipt, and for Solana native currency SOL transfer/receipt, "Assoc

