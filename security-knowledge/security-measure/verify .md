# How to verify whether the wallet is genuine

### <mark style="color:blue;">**MD5 and SHA256 verification tool**</mark>

File hash verification tool refers to the tool that calculates the hash value of the file content. With these tools, the hash value of the file can be quickly calculated, and compared with the official hash value to verify whether the file content has been tampered with.

### The purpose of MD5 and SHA256 verification

Decentralized self-custody wallet is a platform where we import private keys or mnemonics to manage assets on the chain, so how to select and use the platform is particularly important. As a decentralized self-custody wallet with a large number of users, TokenPocket is naturally "concerned" by lawbreakers. They decompiled the genuine APK and added the settings that can import private keys and mnemonics, and then packaged and released it to other websites to "wait for the victims". Once someone downloads and uses the wallet through a search engine or recommendation by others, his private key and mnemonic will be leaked and all assets will be lost.

Judging from the recent feedback from emails and communities, the cases of stealing through fake wallets have increased. That is why we have made this tutorial. By verifying the MD5\SHA256 value on PC and mobile platforms with online tools, we hope to improve everyone's security awareness and learn to use tools reasonably to protect their assets on the chain.

Please be sure to enter the only official website address of TokenPocket: [www.tokenpocket.pro](https://www.tokenpocket.pro)

### The difference between MD5 and SHA256 algorithms

Common points:

1. Both are cryptographic hash functions, and the encryption is irreversible.
2. Both can encrypt objects of any length, and neither can prevent collisions.

As for security

1. SHA256 (called SHA2) is the most secure, but takes more time than the others.
2. MD5 is relatively easy to collide, and not so secure.

### MD5 and SHA256 parameters of the official wallet APK:









### The online tools to verify MD5 and SHA256

There are many tools for online verification of MD5\SHA256 value, and their usage is similar. You only need to drag or load the apk file downloaded to the PC into the verification platform to wait for the result. The obtained result can be verified by comparing it with the MD5 or SHA256 value of the genuine APP published on the official website of TokenPocket<mark style="color:red;">(There may be advertisements and other content in the online tool page, please use the main verification function, and do not recommend anything else).</mark>

Tool 1: Open the link https://www.dute.org/file-hash-validator to select the hash algorithm, usually MD5 is widely used, and the safest algorithm is SHA256. You can also try other hash algorithms. After selecting or dragging the downloaded APK file at the top, the result will be quickly obtained at the bottom. You only need to copy the result and compare it with the officially announced MD5 or SHA256 hash value to complete the verification.
