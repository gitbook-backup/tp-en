# Account Abstraction

From the 64 hexadecimal characters composing the private key of a Bitcoin address in 2009 to the introduction of the secret recovery phrase concept into the blockchain with the Bitcoin Improvement Proposal 39 (BIP39) in 2013, private keys and secret recovery phrase as the most crucial information for protecting user assets have continued to evolve in the blockchain for a decade. In 2020, Vitalik Buterin’s [EIP-2938: Account Abstraction](https://eips.ethereum.org/EIPS/eip-2938) proposed a more comprehensive and detailed concept of Account Abstraction. Since then, Account Abstraction wallets have begun to develop.

### <mark style="color:orange;">**How to “bring the next billion users into Web3.0”?**</mark> <a href="#b7a6" id="b7a6"></a>

Perhaps the Account Abstraction wallets brought about by the concept of Account Abstraction could be one direction.

### Key Words <a href="#b991" id="b991"></a>

**Account Abstraction** is a blockchain technology that allows users to use smart contracts as their accounts, aimed at enhancing the management and interaction flexibility of Ethereum accounts (EOA accounts).

**EOA Wallet**, Externally-Owned Account, is controlled by a private key and secret recovery phrase, currently the largest user-volume traditional wallet.

**AA Wallet,** Account Abstraction Wallet, based on the ERC-4337 protocol is a type of smart contract wallet.

### <mark style="color:orange;">The Limitations Of EOA Wallet.</mark> <a href="#df3f" id="df3f"></a>

Do you still remember the first time you used an EOA wallet(e.g. TokenPocket, MetaMask.)

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*9Hwa3UV32qaKXPvrNLG1_w.png" alt="" height="444" width="700"><figcaption></figcaption></figure>

The limitations of EOAs,

> **1. Assets are controlled by private keys and secret recovery phrases.**

EOA wallet is the general term for the most common wallet account system. The EOA wallet is solely controlled by the private key and secret recovery phrase. Users must securely store the private key and secret recovery phrase of the EOA wallet. Once leaked, it will lead to the loss of wallet assets.

For all crypto users, this is a security challenge. In the past, we have introduced several products to solve the security of private key and secret recovery phrase storage, such as [hardware wallets](https://keypal.pro/), [cold wallets](https://medium.com/@tokenpocket-gm/unleashing-the-power-of-cold-wallets-98f09a47a2c6), [multisig wallets](https://medium.com/@tokenpocket-gm/a-new-tip-for-protecting-your-crypto-create-a-multisig-wallet-on-tokenpocket-2a35a9a7746e), etc. However, these are more difficult for newbies to use and its core still relies on the storage and usage of private keys and secret recovery phrases.

> **2. The interaction logic is not user-friendly.**

* High and unstable on-chain gas fees.
* Multiple factors affect transaction confirmation.
* Complex transaction processes.

Taking Ethereum as an example, to execute a transfer or transaction on the Ethereum network, you must pay the native token ETH as a gas fee to get the transaction confirmed on the chain. If a user’s wallet does not have ETH, the only option is to purchase it through a centralized exchange or through a third-party cross-chain bridge and then transfer it to the wallet. In special cases, due to congestion on the network, there can be an increase in gas fees or transaction failures, resulting in losses for users.

The limitations of the EOA wallets mentioned above are challenges that all newbies currently face. To solve these challenges, significant knowledge acquisition and supplementation are required, along with facing challenges such as “risk approvals” and “risky tokens” during the learning process.

The introduction and development of the “Account Abstraction” concept have, to some extent, addressed these issues.

### <mark style="color:orange;">How to define Account Abstraction?</mark> <a href="#9eb0" id="9eb0"></a>

“Account Abstraction” refers to the “abstraction” of the wallet itself. In addition to the familiar abstraction processing of “private key and secret recovery phrase”, it also includes the abstraction processing of account interaction processes, user experiences, and on-chain experiences.

From a technical perspective, “Account Abstraction” refers to the complete control of the account by smart contracts, with certain contract details being an “abstract” concept for the Ethereum protocol. Each account is a smart contract, allowing users to freely control smart contract accounts without needing to handle any private key or secret recovery phrase.

From a user perspective, “Account Abstraction” has led to significant enhancements and optimizations in account interaction details, making the wallet usage process more convenient and improving the applicability of Web3.0.

We will introduce “Account Abstraction” from four main aspects: “Social Recovery”, “Signature Abstraction,” “Gas Fee Abstraction,” and “Nonce Abstraction.” To better understand “Account Abstraction,” we will also use more comprehensible examples during the introduction.

> **1. Social Recovery**

“How to back up the private key and keep my assets safe?”

That’s the most common question asked by users, and also the most significant user pain point with current EOA wallets.

Account Abstraction abstracts the private keys and secret recovery phrases, eliminating the need for users to back up private keys and secret recovery phrases during the wallet creation process. If the wallet is accidentally uninstalled or the wallet account is deleted, the account can be recovered through multi-factor authentication and social recovery (such as email).

> **2. Signature Abstraction**

Today, transactions from your EOA wallet require a signature generated by your wallet’s private key using the [Elliptic Curve Digital Signature Algorithm (ECDSA)](https://ethereum.org/en/glossary/#ecdsa) to be valid. In other words, a private key is the sole proof to control your wallet assets. Account Abstraction separates the ECDSA, allowing users to customize rules to approve the transaction that is initiated by the wallet. In simple terms, you, are the sole credential controlling the assets.

Here are the explanations of Signature Abstraction through the functionalities of “Transaction Limits,” “Multi-Party Approvals,” and “Auto Payments”:

a) Transaction Limits: If the value of a signature exceeds your preset limit, the wallet associated with your smart account can decline the transaction or request additional.

e.g. You will bind your credit card to pay the daily or monthly household expenses, if it exceeds the limit, your bank account will refuse the transaction (or contact you to confirm the payment at once).

b) Multi-Party Approvals: You can delegate partial control of the wallet to trusted parties, we can call them “guardians”. “Guardians” could be friends, family, service providers, or even a separate device you own, such as the KeyPal hardware wallet. Consequently, “guardians” have the approval to control the assets in your account.

e.g. [TokenPocket MultiSig wallet](https://medium.com/@tokenpocket-gm/a-new-tip-for-protecting-your-crypto-create-a-multisig-wallet-on-tokenpocket-2a35a9a7746e) is one of the concepts of “Account Abstraction”.

c) Auto Payments: You can authorize third-party services to “withdraw” assets from your account to support a specific recurring expense.

e.g. Back to the credit card example, you can also bind your AA wallet to pay the payment(e.g. pay for a subscription to a platform). For sure, you need to confirm the platform accepts the crypto payment method.

“Transaction Limits,” “Multi-Party Approvals,” and “Auto Payments” are the three prominent application scenarios in signature abstraction. We will also introduce more usage scenarios in the future, combining new AA wallet features, to integrate the AA wallet into your Web3.0 life.

> **3. Gas Fee Abstraction**

As mentioned before, any transaction on the Ethereum wallet must pay the native token ETH as a gas fee to push the transaction on the chain. This type of interaction logic is not user-friendly, especially for new Web3.0 users, as the process of obtaining miner fees is overly complex. Account abstraction can effectively solve this problem.

In the account abstraction system, the smart contract account created by the user can use other ERC-20 tokens to pay the gas fee on their behalf. At the contract level, there will be a “relay” to convert ERC-20 tokens into native ETH, thus pushing the transaction on the chain.

In the future, projects can even achieve “feeless interaction” at the user level by donating or sponsoring fees through the relay, truly achieving the same convenient transactions as Web2.0.

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*bdJqCtG7IBI99y1fKLwe8Q.png" alt="" height="444" width="700"><figcaption></figcaption></figure>

> **4. Nonce Abstraction**

In the Ethereum system, Nonce is an important concept used to ensure that transactions are executed in a specific order. The purpose of Nonce is to maintain the order and integrity of transactions to prevent “replaying” attacks and disorderly transaction execution.

If you need to initiate two or more transactions, and the Nonce values of these transactions are 0 and 1, respectively, you must wait for the transaction with Nonce=0 to be executed/confirmed before executing the transaction with Nonce=1. For users who need to perform batch transaction operations, such a process is too rigid, leading to low work efficiency.

Account Abstraction allows you to create a custom replay protection mechanism (instead of the Ethereum protocol enforcing strict transaction ordering). For example, it is possible to use Nonces that allow batch processing of multiple transactions, thus pushing multiple transactions onto the chain. This solves the problems caused by specific order requirements, making Web3.0 more lightweight.

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*j_GvzoAjidjkqtAkoVk5LA.png" alt="" height="444" width="700"><figcaption></figcaption></figure>

**So, what will be the interaction process for AA wallets?**

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*QIHN6BqE_y-tfEoM59qfHQ.png" alt="" height="444" width="700"><figcaption></figcaption></figure>

### <mark style="color:orange;">**Conclusion**</mark> <a href="#f34e" id="f34e"></a>

Account abstraction stands as one of the best solutions to address the limitations of EOA wallets, bringing increased flexibility and operability to the field of wallets. TokenPocket will launch the AA wallet soon, bringing users more possibilities in the Web3.0 realm.
