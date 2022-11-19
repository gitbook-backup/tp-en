# How to create a MultiSig Wallet?

## **What is a MultiSig wallet?**

Generally, all the on-chain operations need to sign by private key, and the private key signature is equivalent to the process of permission verification. The wallet is divided into single-sig wallet and multi-sig wallet. The single-sig wallet is controlled by a private key. For example, the common wallet we use at present is the single-sig wallet. The multi-sig wallet is jointly controlled by 2 or more private keys. The private keys holders of the multi-sig wallets are the managers.&#x20;

Therefore, when the multi-sig wallet needs to execute the on-chain operation, the managers need to sign according to the weight.

The ETH/ERC20(Including the EVM-based chains like BSC/BEP20, etc.) MultiSig wallet using the smart contract to sign.



**Application scenario:**

1\. Manage assets by multiple persons to avoid the misappropriation of assets by individuals;

2\. Perform multi-address signature management for assets to enhance asset security.

3\. Other security scenarios.

\


## **Create a MuitiSig wallet**

1. Open TokenPocket and click \[No wallet] for the first time, and choose \[MultiSig Wallet]. You can also click the upper right corner to create a multisig wallet.



2\. You need to choose the network before you create a multisig wallet, please read the reminders carefully during the creation process and then click \[Next Step].



3\. The steps of creating a multi-signature wallet are the core content. The following figure shows each type of content as follows:

\[Wallet Name] is as same as the wallet name you created before, which can be customized and it won’t execute on-chain.

\[Owners] is to set to management wallets of the multisig wallet. The owners can manage and control the multisig wallet and a maximum of 30 owners can be set, which can be understood as the \[Threshold Setting] of the multisig wallet. The owners can be set up flexibly, it is suitable for enterprises, DAO, and individuals.&#x20;

\[Required Signatures] it’s also called Weight, the difference between EOS/TRON multisig wallets and EVM multisig wallet is that EOS/TRON multisig wallets’ weights can be set as 1 or greater, while EVM-based multisig wallets’ weights can only be set as 1.&#x20;

\[Payment Details] The multisig scheme of EVM-based chain is a smart contract, so creating a multsig wallet requires paying Gas (miner's fee), which TokenPocket does not charge.\
\[Pay with] You can click and select the wallet address imported in the wallet to pay the Gas (miner's fee) fee.

After everything is set, click \[Confirm] to read the reminders for the creation of the multisig wallet. You can also read the information of this creation on the blockchain explorer.

\


4\. There are two states of multisig wallet creation are success and failure. It will be affected by node, network, Gas (miner's fee), etc. Therefore, if we see the situation of creation failure on the right of the picture below, we only need to click \[Delete] displayed in the interface to delete the failed multisig wallet creation.



5\. After you’ve successfully create a multisig wallet, click \[Details] and you can see the \[Transaction Queue] and \[Manage].



6\. \[Transaction Queue] will display the generated multisig order, you can click and complete the order; You can view information such as \[Required signatures], \[Latest Nonce on-chain] and \[Associated Wallet] in \[Manage], the associated wallet is the owners. If there is an address that has not been imported, you can click \[Import] and use the private key or secret recovery phrase to import it. Whether the associated wallet is imported will affect the transaction and the use of DApps.

\


To sum up, the multisig wallet on the EVM-based chain is a smart contract. Creating a multisig wallet does not require to back up the secret recovery phrase or private key, does not require to set a password, does not require complex code, and is similar to the watch wallet.

The key point of creating a multisig wallet is the reasonable setting of \[Owners] and \[Required signatures]. A reasonable setting of the multisig wallet can play its maximum security and convenience. The commonly used multiple signatures are 2/3, 3/5, and so on, which need to be selected according to the individual situation.
