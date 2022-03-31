# FAQs on Bitcoin Wallet

**1. Why is the fee so high for bitcoin transfer?**

Because bitcoin is only one megabyte in each block, and can only handle five transactions per second, miners' fees have risen since the volume of transactions has increased.

**2. Why does my USDT prompt an address error when I want to transfer to a bitcoin address?**

The bitcoin-based USDT (issued under the Omni protocol) and ethereum-based USDT (issued under the erc-20 protocol) cannot transfer to each other.

When transferring USDT, you can tell whether the USDTs are based on the same protocol by their address starting numbers: the USDT issued under Omni protocol starts with "1", and the USDT issued under erc-20 protocol starts with “0x".

**3. Can USDT transfer to my bitcoin address?**

Yes

**4. How many bitcoin addresses can you create in the TokenPocket wallet?**

You can create as many as you want, and it's free.

**5. Can I create multiple BTC addresses?**

Depending on your needs, you can create as many as you want.

**6. My bitcoin has been transferred out but the receiver said did not receive, what should I do?**

You can query in the blockchain browser, maybe the queue delay is more severe. The speed is really so slow when there are more transactions.

**7. Can the TP wallet automatically collect bitcoins?**

This function will be designed later, welcome to give valuable advice.

**8. How to choose the best miner's fee for bitcoin?**

Bitcoin miners fee calculation: = Fees (satoshi/byte) \* Site (byte) (\* satoshi = sat, 1 bitcoin = 100 million satoshi), you can go to https://bitcoinfees.earn.com to view the data to get the best miner's fee.

For ordinary users, we generally use the default recommended miner's fee in the wallet (such as TokenPocket), of course, we can also flexibly turn on the advanced mode to make free settings.

**8. What is the proof of work (POW)?**

The most commonly used technical principle for POW is the hash function. Since any value n of the input hash function h() will correspond to an h(n) result, and as long as n changes one bit, it will cause an avalanche effect, so it is almost impossible to push back from h(n) to n, so by specifying to find the characteristics of h(n), let the user do a lot of exhaustive operations, can achieve proof of work. In short, it is through a certain amount of work (mining) to get the corresponding reward (Token).

**9. What are the advantages and disadvantages of the bitcoin lightning network?**

Lightning networks can provide significant improvements in scalability, and transaction speeds and transaction rates should be significantly improved without affecting the underlying security of the core protocols. However, there are always two sides to everything. Let's take a look at the advantages and disadvantages of lightning networks.

Advantages of the lightning network:

Fast payments: payments within a given channel can be almost as fast as data being transferred between two nodes over the Internet.

No trusted third party is required: the two participants in the channel pay each other directly using regular bitcoin transactions, and no third party controls their funds.

The payment channel can remain open indefinitely: as long as the two parties in the channel continue to work with each other, the channel can remain open indefinitely.

Across the blockchains: the payment channel can be routed across multiple blockchains if another blockchain supports the same hash function for the hash lock and has the ability to create a time lock.

Disadvantages of the lightning network:

The security of lightning network payment may make the lightning network not suitable for a large payment. The payee needs to sign the recovery transaction before receiving the payment, and a hot wallet is needed to receive the payment, which means there is a risk that the private key will be exposed if a security incident occurs.

**10. What is the relationship between USDT on BTC and BTC?**

USDT (full name Tether USD). It is a stablecoin issued by Tether, formerly known as Realcoin, which is registered in the isle of man and Hong Kong. USDT is the stable currency with the highest market share on the market. It was originally issued as a cryptocurrency based on the Omni protocol, which can be simply understood as the USDT based on bitcoin.

Omni-USDT is stored on the bitcoin address, so the type of fee to be paid for each transfer is bitcoin. The address is 1 or 3 at the beginning, for example, 1NTMakcgVwQpMdGxRQnFKyb3G1FAJysSfz. It is important that to successfully transfer Omni-USDT on the blockchain, there must be at least 0.0002 bitcoins in the address. At the same time, for each Omni-USDT transfer, a small amount of BTC transfer will be generated accordingly. In other words, when we made an Omni-USDT transfer on the blcokchain, two transfers "Omni-USDT and small BTC" actually took place.

Tip: there are currently BTC, ETH, TRX, and EOS that support the USDT.

**11. What is the bitcoin lightning network?**

Lightning network is a distributed network that enables instant payment across the participant network through the smart contract function, while taking advantage of the blockchain feature to eliminate the risk of hosting funds to third parties. Mainly used for instant, high-volume micropayments. In essence, it is to set up another channel outside the bitcoin main chain, where users' digital currency can make quick payments, because the lightning network is a decentralized architecture, which is fundamentally different from traditional exchanges.

**12. Does a bitcoin address have to start with a number?**

No, there are 1, 3, and bc1, which represent the following:

The address at the beginning of 1 is P2PKH(pay-to-public-key-hash) address, which is the original address, and is called ordinary BTC address;

The address at the beginning of 3 is P2SH(pay-to-script-hash) address, and the internal address also needs to be segwit, that is, the segwit address.

The address at the beginning of bc1 is a BECH32 encoded address, an address format developed specifically for segwit, and an segwit address.

The address at the beginning of 3 and bc1 are smaller and less expensive than that of 1, which can improve the packaging speed of BTC block.

**13. How many bits is the bitcoin address?**

The length of a typical BTC address is 26-34 bits. It's worth noting that the address of the bitcoin is not the public key, but the hash of the public key. That is, the address can be derived from the public key, but the public key cannot be deduced from the address, because the hash function is a one-way function.

Tips：

The address at the beginning of 1 is P2PKH(pay-to-public-key-hash) address, which is the original address, and is called ordinary BTC address;

The address at the beginning of 3 is P2SH(pay-to-script-hash) address, and the internal address also needs to be segwit, that is, the segwit address.

The address at the beginning of bc1 is a BECH32 encoded address, an address format developed specifically for segwit, and an segwit address.

The address at the beginning of 3 and bc1 are smaller and less expensive than that of 1, which can improve the packaging speed of BTC block.

The BTC address of Satoshi Nakamoto: 1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa

**14. What is the smallest unit of bitcoin?**

The traditional currency we use every day can be broken down into cent, so for bitcoin there is also its smallest unit, satoshi. How small is satoshi? 1 satoshi = 0.00000001 BTC.

In October 2019 satoshi, bitcoin's smallest unit, was added to the Oxford English Dictionary. This is the latest addition to the famous English vocabulary, and it's part of the encryption industry's terminology, but it's not the first. In 2013, the OED added the word "bitcoin" defining it as "a digital currency that can be traded without a central bank”.

**14. Will the miner's fee be deducted if the BTC transfer fails?**

In the bitcoin network, the transfer requires the miner to package the transaction. But if the deal fails for reasons such as a lack of miners' fee, since the deal has been packaged by the miners, the miner's fee will be deducted and not refunded to the user's account. This is also a feature of the consensus algorithm of POW (Proof Of Work).

15\. How to export the BTC private key of TokenPocket wallet?

The public key in the BTC is used as a collection address. The private key is known only to you, if it is public or lost means that your assets will be lost. Therefore, the private key plays an important role in our assets. Although the registration of the TokenPocket wallet started as a reminder of backup and verification mnemonic(equally important), the backup of the private key means that we can have more controllable keys. If one of the two is lost, the asset will not be lost.

The steps to export the private key through TP wallet are as follows: open the wallet -- click the blank at the top of the receipt -- select export the private key in the pop-up menu -- enter the password for authorization to record and save the private key (the QR code is for convenient transfer through different devices, please be sure to use it in a safe environment).

**16. What is BTC segwit?**

Segwit is a method of blockchain expansion that has been successfully implemented in litecoin and bitcoin. At present, each block on the blockchain not only records the specific information of each transfer transaction, that is, how many bitcoins were received or transferred from the account at which point, but also contains the digital signature of each transaction to verify the legitimacy of the transaction.

When the miners package the blocks, they need to verify each transaction with a digital signature, confirm that there is no problem, and then record the transaction in the block. But for the average user, he only cares about how many assets are in each account and does not need to verify every transaction. Segwit is the digital signature information in the block out, so that each block can carry more transactions, thus achieving the purpose of expansion.

Advantages of segwit:

More secure, with better security than common addresses.

Faster, scalable block capacity, faster checking of transactions.

Cheaper, transaction fees are cheaper than regular address types.

How to identify the segwit address:

Most addresses of the segwit start with "bc", while ordinary addresses start with "1", and "3" may multiple signature addresses or the segwit address used for transitional period.

**17. Bitcoin transfer is slow, can it be accelerated?**

BTC transfer is slow, mainly because the transfer fee is less, so you can increase the amount of miner fee on the transfer page to get faster transfer speed.

**18. How to import the BTC private key into the wallet?**

Step 1: click "add wallet"

Step 2: click "Private Key"

Step 3: enter the private key and wallet password, click "I agree" and "Import it”.

**19. How to set the miner fee of BTC?**

Miner's fee reference: In the bitcoin browser: https://btc.com/stats/unconfirmed-tx,Home page - statistics - unconfirmed transaction page will display the current best handling fee, you can follow this value to set.

In the TokenPocket wallet transfer page, you can set the miner's fee number manually, or you can use the miner's fee recommended by the wallet by default.

**20. How to transfer BTC to exchange by wallet?**

Step 1: click "Transfer" on the asset page.

Step 2: click "Transfer".

Step 3: enter the address and quantity of the BTC and click next to enter the password.

**21. How to delete the BTC wallet?**

Step 1: go to the wallet details page and select "delete".

Step 2: enter the wallet password for verification to complete the wallet deletion.

Please make sure to save the private key before deleting the wallet.

**22. What if you lose your password to your bitcoin wallet?**

There are two options, you can choose to reset the password on the wallet details page, or you can choose to delete the wallet and reimport the private key or mnemonic. Whoever holds the private key and mnemonic is the owner of the wallet.

**23. How to reset the password of the bitcoin wallet?**

Step 1: on the wallet list page, click on the pinion (to go to the wallet details page). You can also click on the assets home page, the blue banner to enter the details page.

Step 2: on the wallet details page, select modify password.

Step 3:If you remember your old password, you can change it directly.

**24. What if the BTC private key is lost?**

Case 1: the phone or computer now has this BTC wallet, and remember the password, you can enter the password in the wallet details to export the private key or mnemonic.

Case 2: the wallet APP has been uninstalled and the private key is not backed up. In this case, the private key cannot be retrieved.

**25. How to backup bitcoin private key?**

Best solution: print ten copies of the mnemonic when there is no camera and you have only yourself with you. Put them in a plastic bag to keep them dry. Keep them in a safe place.If possible, you can also laser etch them on the stainless steel plate.

The next best solution: you can copy them manually, be case-sensitive, and keep them neat. To be careful, you can copy them twice and store them in a plastic bag in a safe place.

Other networking situations, cloud storage, or stored in the phone album are likely to be lost or stolen.

**26. How to create a BTC wallet in TokenPocket?**

Step 1: on the "assets" page, select "create wallet" and then select "bitcoin".

Step 2: select "create wallet".

Step 3: take the name of the wallet yourself, password 8 digits and letters, and then click "create wallet".

Step 4: click "backup wallet".

Step 5: back up your mnemonics, preferably in a camera-free place, and print them out for safekeeping. Screenshots are easy to lose, physical preservation is the safest. Click "next step"after backup

Step 6: click the backup mnemonic words in order, click all finished, click "finish".

Now the BTC wallet is created.

**27. How to change the name of bitcoin (BTC) wallet in the TokenPocket wallet?**

Step 1: click "mine" to go to the personal center page and click "manage wallets".

Step 2. Click the bitcoin menu to enter the wallet you want to modify.

Step 3. Go to the wallet details page and click the modify button next to the wallet name to modify

**28. Is there a bitcoin browser in the TokenPocket wallet? How to use it?**

Yes. The method is as simple as clicking on the "blockchair" at the top of the wallet "assets" page.

**29. When my TokenPocket wallet APP was disconnected, someone transferred BTC bitcoin to me. Can I receive it?**

Yes. Bitcoin (BTC) will appear in your account the next time you open the wallet program after connecting to the Internet. Bitcoins are not actually received by the wallet software, they are added to a public ledger shared by all the devices on the network.

If someone transfers BTC to you when your wallet is not running, the wallet will download the block data and update any unrecorded transactions when you open your wallet later, and the BTC record of the transfer will appear in the wallet.

**30. Will I lose my bitcoin stored in my TokenPocket wallet? Will my wallet steal my BTC?**

No. Strictly speaking, whether you lose your bitcoin in your wallet depends on whether your private key is lost or stolen. As a decentralized wallet, the TokenPocket wallet does not store the user's private key, so there is no permission to transfer the user's assets. Please keep your private key safe.

**31. What coins are on the BTC network?**

Unlike ETH, EOS and other public blockchains which support the development of smart contracts, the bitcoin network currently only have BTC and USDT. The USDT is known as OMNI (if you see it on an exchange). Some users may mention fork coins such as BCH, but they are not part of the bitcoin network.

**32. Can I mine BTC bitcoin with the TokenPocket wallet?**

As a decentralized wallet, TokenPocket has no mining function. However, you can purchase bitcoin cloud computing products provided by a third party on the TokenPocket wallet for cloud mining

**33. Will it give me interest if I deposit BTC in the TokenPocket wallet?**

TokenPocket as a decentralized wallet, your BTC assets are stored on the blockchain, and the wallet is only used as a management tool to synchronize the data information on the blockchain. So BTC is not stored in the wallet, which does not charge users any fees or provide any interest.

**34. Where is the price of BTC in the TokenPocket wallet displayed according to?**

According to the market site CoinMarketCap (https://coinmarketcap.com/) real-time BTC display price.
