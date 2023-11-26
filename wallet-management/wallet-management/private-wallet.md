# How to Use the Private Wallet?

The private wallet is implemented through the application lock feature in the wallet. After enabling the application lock, you can add a \[subspace], which is the privacy space. After setting a password in the privacy space, you will enter a completely new \[create wallet] \[import wallet] interface.

After importing or creating a wallet, the next time you open the wallet, you will enter a different private wallet based on the password you entered. For example, if you set password 1 in subspace 1 and password 2 in subspace 2, entering the respective subspace password will open the wallet interface for that subspace.

This setting provides better private but requires remembering the password. If you forget the password, you can only recover assets on the chain using the key.

**TP Wallet version 2.1.7 already supported the private wallet, and Android support will be available soon.**

### Private Wallet Use Guide: <a href="#0" id="0"></a>

1. Open TP Wallet, click \[Me], and select \[Security].

<figure><img src="../../.gitbook/assets/image (71).png" alt=""><figcaption></figcaption></figure>

2. Click on \[App Lock], toggle the switch for \[Activate].

<figure><img src="../../.gitbook/assets/image (72).png" alt=""><figcaption></figcaption></figure>

3. Set a password in the interface, with a minimum requirement of 8 characters. It is recommended to create a slightly complex password and remember it, as it will serve as the passphrase for the current wallet. Once the password is created, you will see the option to \[Add Subspace].

<figure><img src="../../.gitbook/assets/image (73).png" alt=""><figcaption></figcaption></figure>

4. After clicking on \[Add Subspace], you will see a prompt interface. Click on \[Start Creating], customize a space name, and click on the \[Next] step.

<figure><img src="../../.gitbook/assets/image (74).png" alt=""><figcaption></figcaption></figure>

5. Here, you also need to set a password, which is the access password for the newly created sub-space. Please be sure to remember this password. After completing the password setup, click on \[Enter Space].

<figure><img src="../../.gitbook/assets/image (75).png" alt=""><figcaption></figcaption></figure>

6. In the new-created subspace, you need to create or import a wallet again based on your needs. After completing the operation, the next time you open the wallet, you can enter the corresponding wallet by entering the password for the different subspace we set.

<figure><img src="../../.gitbook/assets/image (76).png" alt=""><figcaption></figcaption></figure>

### Q\&A:

Q: Can the passwords for different subspaces be the same?&#x20;

A: No, the passwords for different subspaces must be unique. The entry into a subspace depends entirely on the set password, and there will be prompts in the interface.

Q: If I close the application lock for a subspace, will the data of other subspaces be lost?&#x20;

A: No, closing the application lock for the current subspace will keep the wallet in the currently accessed wallet. If you need to access another sub-space, you'll need to reopen the application lock and open the wallet again to enter the password for a different sub-space.

Q: Do I need to save the key for each subspace?&#x20;

A: Yes, it still needs to be saved. Essentially, it is still an externally owned account (EOA) type of key wallet, so be sure to backup your private key or mnemonic phrase offline.
