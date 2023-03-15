# How to create/import a MultiSig wallet in TP Extension Wallet?

## <mark style="color:orange;">About MultiSig wallet:</mark>

Corresponding to the multi-signature wallet is the single-signature wallet. If we want to conduct a transfer operation on the blockchain, we need to generate a signature with the wallet. We sign and send the transaction out. This is the way for a typical single-signature wallet and it is also for our usual wallet.

A multi-signature wallet, as the name suggests, is a wallet that requires multiple people to sign in to perform an operation. Transferring with a multi-signature wallet often requires >= 1 person to sign and send the transaction before the operation can be completed. When using a multi-signature wallet, we can specify the signature mode of M/N, that is, only M signatures among N persons can complete the operation. For example, the 2/3 signature mode means that two of the three people can sign.

The multi-signature of ETH/ERC20 (including EVM chains such as BSC/BEP20) adopts a lightweight smart contract method.

#### Applicable scenes:

1、When managing assets by multiple people to avoid assets being misappropriated by individuals;

2、Multiple encryptions of assets through multi-signature to enhance asset security;

3、Other security application scenarios.

## <mark style="color:orange;">Create a MultiSig wallet in TP Extension</mark>&#x20;

1. Open TokenPocket Extension, click the menu in the upper right corner and click MultiSig wallet.

<figure><img src="../../../.gitbook/assets/组 26.png" alt=""><figcaption></figcaption></figure>

2. You can select \[Create Wallet] or \[Impor Wallet] on this page.

<figure><img src="../../../.gitbook/assets/image (14) (1) (1).png" alt=""><figcaption></figcaption></figure>

3.  The steps of creating a multi-signature wallet are the core content.&#x20;

    **\[Wallet Name]** is as same as the wallet name you created before, which can be customized and it won’t be recorded on chain.

    **\[Owners]** is to set the managers of the multisig wallet. The owners can manage and control the multisig wallet and a maximum of 30 owners can be set, which can be understood as the \[Threshold Setting] of the multisig wallet. The owners can be set up flexibly, it is suitable for enterprises, DAO, and individuals.&#x20;

    **\[Minimum number of confirmations]** Set the minimum number of the MultiSig wallet. When the minimum number sign, on-chain operations such as transfer and contract interaction can be initiated. You are advised to set the minimum number of confirmation signatures to a value greater than 2.

    **\[Estimated fee]** The multisig scheme of an EVM-based chain is a smart contract, so creating a multsig wallet requires paying Gas (miner's fee), which TokenPocket does not charge.\
    **\[Pay with]** You can click and select the wallet address imported in the wallet to pay the Gas (miner's fee) fee.

    After everything is set, click \[Confirm] to read the reminders for the creation of the multisig wallet. You can also read the information on this creation on the blockchain explorer.

<figure><img src="../../../.gitbook/assets/组 28.png" alt=""><figcaption></figcaption></figure>

4. You can view the statue of Creation.

<figure><img src="../../../.gitbook/assets/image (31) (1).png" alt=""><figcaption></figcaption></figure>

5. After creating successfully, click \[Enter Wallet], then you can view your MultiSig wallet.

<figure><img src="../../../.gitbook/assets/image (14) (1).png" alt=""><figcaption></figcaption></figure>

## <mark style="color:orange;">Import a MultiSig wallet in TP Extension</mark>

1. Open TokenPocket Extension, click the menu in the upper right corner and click MultiSig wallet.

<figure><img src="../../../.gitbook/assets/组 26.png" alt=""><figcaption></figcaption></figure>

2. You can select \[Impor Wallet] on this page.

<figure><img src="../../../.gitbook/assets/image (26) (1) (1).png" alt=""><figcaption></figcaption></figure>

3.  Select the network and enter your MultiSig wallet address, then click \[Import].

    <figure><img src="../../../.gitbook/assets/image (18) (1).png" alt=""><figcaption></figcaption></figure>

