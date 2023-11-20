# Page

An HD wallet, short for Hierarchical Deterministic wallet, is designed for decentralized management of private keys and assets. The digital assets (Tokens) we possess are recorded on the blockchain. Over time, for the purpose of achieving different functionalities and convenient operations, wallets such as cloud wallets and HD wallets have been developed. HD wallets, in particular, not only prioritize security but also facilitate the creation of sub-private keys as part of the hierarchical deterministic wallet type.

In reality, understanding the concept of hierarchical deterministic wallets is not as challenging as one might imagine. Its principles can be expressed in two sentences: Firstly, a random number is used to generate the master private key, which is no different from the process of generating private keys in other wallet types. Then, a deterministic and irreversible algorithm is used to generate any number of child private keys based on the master private key.

Why use a "deterministic, irreversible" algorithm? Because "deterministic" ensures that all child private keys can be generated from a single master private key, and "irreversible" ensures that the master private key cannot be reverse-engineered from the child private keys.

It is called a hierarchical deterministic wallet because the structure of private key derivation is tree-shaped. The parent key can derive a series of child keys, each child key can further derive a series of grandchild keys, and so on, leading to an infinite derivation.

<figure><img src="../../.gitbook/assets/image (70).png" alt=""><figcaption></figcaption></figure>
