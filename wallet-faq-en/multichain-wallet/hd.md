# What is a HD Wallet?

An HD wallet, short for Hierarchical Deterministic wallet, is designed for decentralized management of private keys and assets. The digital assets (Tokens) we possess are recorded on the blockchain. Over time, for the purpose of achieving different functionalities and convenient operations, wallets such as cloud wallets and HD wallets have been developed. HD wallets, in particular, not only prioritize security but also facilitate the creation of sub-private keys as part of the hierarchical deterministic wallet type.

In reality, understanding the concept of hierarchical deterministic wallets is not as challenging as one might imagine. Its principles can be expressed in two sentences: Firstly, a random number is used to generate the master private key, which is no different from the process of generating private keys in other wallet types. Then, a deterministic and irreversible algorithm is used to generate any number of child private keys based on the master private key.

Why use a "deterministic, irreversible" algorithm? Because "deterministic" ensures that all child private keys can be generated from a single master private key, and "irreversible" ensures that the master private key cannot be reverse-engineered from the child private keys.

It is called a hierarchical deterministic wallet because the structure of private key derivation is tree-shaped. The parent key can derive a series of child keys, each child key can further derive a series of grandchild keys, and so on, leading to an infinite derivation.

<figure><img src="../../.gitbook/assets/image (70).png" alt=""><figcaption></figcaption></figure>

This structure is very similar to the organizational hierarchy of a company and a family tree!

When we first create an HD wallet or back up a wallet, a mnemonic phrase is generated. The mnemonic phrase consists of a sequence of English words, and this sequence of words can create a seed, which in turn can generate all the private keys. The word order also serves as the backup for the wallet and can be used to restore it. The seed corresponds to the random number of the deterministic wallet.

The advantage of an HD wallet is that it only requires the master public key to generate any number of child public keys. In other words, new (public key) addresses can be generated based on the master public key without the involvement of private keys (master private key and child private keys). These addresses can still be controlled by the master private key.

With advantages come disadvantages; when we expose the mnemonic phrase, the assets are exposed to significant risks.
