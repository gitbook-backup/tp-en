# How to verify whether the wallet is genuine

### <mark style="color:blue;">**MD5 and SHA256 verification tool**</mark>

File hash verification tool refers to the tool that calculates the hash value of the file content. With these tools, the hash value of the file can be quickly calculated, and compared with the official hash value to verify whether the file content has been tampered with.

### <mark style="color:blue;">The purpose of MD5 and SHA256 verification</mark>

Decentralized self-custody wallet is a platform where we import private keys or mnemonics to manage assets on the chain, so how to select and use the platform is particularly important. As a decentralized self-custody wallet with a large number of users, TokenPocket is naturally "concerned" by lawbreakers. They decompiled the genuine APK and added the settings that can import private keys and mnemonics, and then packaged and released it to other websites to "wait for the victims". Once someone downloads and uses the wallet through a search engine or recommendation by others, his private key and mnemonic will be leaked and all assets will be lost.

Judging from the recent feedback from emails and communities, the cases of stealing through fake wallets have increased. That is why we have made this tutorial. By verifying the MD5\SHA256 value on PC and mobile platforms with online tools, we hope to improve everyone's security awareness and learn to use tools reasonably to protect their assets on the chain.

Please be sure to enter the only official website address of TokenPocket: [www.tokenpocket.pro](https://www.tokenpocket.pro)

### <mark style="color:blue;">The difference between MD5 and SHA256 algorithms</mark>

Common points:

1. Both are cryptographic hash functions, and the encryption is irreversible.
2. Both can encrypt objects of any length, and neither can prevent collisions.

As for security

1. SHA256 (called SHA2) is the most secure, but takes more time than the others.
2. MD5 is relatively easy to collide, and not so secure.

### <mark style="color:blue;">MD5 and SHA256 parameters of the official wallet APK:</mark>

<mark style="color:blue;">**Google Play**</mark>

| Version |                MD5               |                              SHA256                              |
| :-----: | :------------------------------: | :--------------------------------------------------------------: |
|  1.7.4  | a3db8395c1a6f9896032c3f239f94e48 | 1e08dfbfb1ae6f343cc742e1b0bb36f1fc1005439aadc386b215a7765fa39b70 |
|  1.7.3  | 19904e8d6a3a64029e24cb3d1376390b | 683efdffcdcf7463f876f239093f259cbb0d202e7517c9ff7ded722a2e776be6 |
|  1.7.2  | ea468f2ba3ccf4319eeae2fe5c7b07c1 | 3a630581244f49fcd317c363d61d19e265906de8d1b2d6bbd66615832333a61f |
|  1.7.1  | e8d383a622eda37d07933cf80b647fc2 | da92c35440b0ef344b8cbccd543503440649fb0c14e3020c64574b534d39620a |
|  1.7.0  | d441edf5c94e57adab597e3245c1a74a | 6b310e3b8f97e9f36b52adbbe43ddb810e043db4db3fa94644f764ae3768095a |
|  1.6.9  | ec200454c69b687a7b7dd54c59acf56b | b6baf6792caa7baf0b1740f33b23b07e922e8299c7e9c02f53b9f80b7b80ee5a |
|  1.6.8  | 8175797b8739dfd27f6f25a55bdce6d3 | a49f4843269d88445532f982c893a41dc069922b51d4ea9b36a6a9c191a405f1 |
|  1.6.7  | 8c3c5e706f9b03cca0f0458417f202c3 | 8c96b54ea00f8c826e2be84e25b0446864e013de9b270d4fe9b6f60ed40be400 |
|  1.6.6  | 73501df3c495a38b9b2c6ff24eeeba1e | e75e6dd6afcb87bfb78e983be6b2c2eddb42fccba70f6d0bf41cbb87648c121b |
|  1.6.5  | 89ad8d584810046a1b261e8ad555ec82 | ae97bf1f7d3bb5917b46bfeb3d052830c7f5ee584c6486ecbc65e1693f9fe359 |
|  1.6.4  | 951dfeb5d7265fa7c132eeeceb780864 | 3afd9ac7c74424d475bd4cf00ac2b6a662a5ae5a5d562529d3aaf2f4fd729311 |
|  1.6.3  | c60ab2f42f48c379ab36f761daf3589e | b979b36df3839edf51e8c15dbedcf0367359c55008403ebb5b662a473b35f64b |
|  1.6.2  | f8df3cef27738ecd4e195e6fed7fe8d0 | dde7014d51df68b8de3905174c666331c307e1ed96dbe9cd51e0a8da00bc6abd |
|  1.6.0  | 66bceb6daeb4b40f736d15f6b38b0d9e | 003d5141a4f442772a9e8a8ede57b543054b72d746df050aa48d7a5349c3c479 |
|  1.5.9  | 88c4d55959c9da313db6acc73ea0d656 | 59ad89d7dbf09a27b5a37e94dd9063178fbb69614367e5b10dfb3944d266249a |
|  1.5.8  | f744d05688acf4a67509c14639829545 | 0c2fd1998d10f364e83749a12c388f681acc6fad85212c7441a9cb7b54649460 |
|  1.5.7  | a1ef0ae6f7a616a85e3cc2645723b07e | 6ce904535ab4035bf1a4ea5ef001c1f82baf9ead660a880b2b4a2244b48f95d8 |
|  1.5.6  | fe1eed863c1214c508d41293537944e8 | f49e4516c547d2f7a6f4d2a577332d5d63ee0b36ea5a73b7d813452d22b2ce5f |
|  1.5.5  | 10e6d8860e2b0a1253a3fc9a541ac3a9 | 95ca32929a294f90de3a2f62ceb792cc4fa442ee632e5df810a6d2bd8b44325d |
|  1.5.4  | 53936f73be5c90dce02ea06919f29fb0 | d4edad4a5277efc29fc896fcabe71a8f17de1fbf69944e340b52a0709dab9695 |
|  1.5.3  | 24a1df1bc85cdb1c34c780c217ee9c1d | 30d50fc1f9f008bbfb3bb33fd5d04f6dcd6e3fb1c9b37ab5ec1815d6c9391bed |
|  1.5.2  | 938e9252cb21fef1c40fac3c4c9492c6 | dfaf358d6f30ead51b52193a5aab8259fd52ac5d8372b47a97951c799842b988 |
|  1.5.1  | f879845afd51d51fabf42e653011da79 | a4162187fac4a623ab5762d15953ae17e659e3c6fa518615a70d8046d2f01355 |
|  1.5.0  | a951c032f8723cc1711f0d3b3256725d | c7f8b8a603d8725ba1df631cf03f2c63dc4c428b5ffe1f3ae3eec400bf3d121b |
|  1.4.9  | 4b88e2ffa2b3d84fbc2f099e1034fb86 | 37b571b7644e456be7260e3d1d93ce59d9e38f694215c85e29e4a1476b6bf634 |
|  1.4.7  | feab610e82a1ed694d24994487f3e38c | b023f39e496ac6a38cc0ef121470cc7c2142f393c75aea504bc8ab979285dffd |

[<mark style="color:blue;">**www.tokenpocket.pro**</mark>](https://www.tokenpocket.pro) <mark style="color:blue;">**or tpwallet.io**</mark>

| Verison |                MD5               |                              SHA256                              |
| :-----: | :------------------------------: | :--------------------------------------------------------------: |
|  1.7.5  | b963703ad2e2301b1aac4d449dfedb41 | 0496c0ecb5a719a642279a8233405a71e09867e1978d5aed38f6fc45973d057b |
|  1.7.4  | e943ca5b2ff356e9e1fe0133b90a22fb | 81cd881a8c3aace2d76d9247e174db48cec4fe50d2e7e5289c9ff20eaf056b52 |
|  1.7.3  | 1894510ae8b325d148f3a02f2e3f57f8 | 41007ee8cdc96f179a05400ef34aa44d541feda23ebe95b1248b868242625fe9 |
|  1.7.2  | 9262f28f781e61852a34b97d23f6acd1 | 97935dbb3c0ce607a3d0bf8d66fe18d5a17213cef8758a6f067fcf2823bc9db5 |
|  1.7.1  | 39a61a17e5b3b0de501c29ee8d2d5d22 | 3ece643ba4599a00be1ae5f580814dcabaf4daa8f292d21b92c5724a2a28a006 |
|  1.7.0  | e2bbf4e2a9dfb1f52e079028a61f3d7c | d46b6a2d90715dd21329ae071f03b4098eef172eae7cc998fbe4c805c338f7bc |
|  1.6.9  | 357d37f7d57b6e5efb3d43c250272c79 | 2519682c8793e6730aa6fa58b3373995d07b7e1c44da5c740c4254d49b393bd3 |
|  1.6.8  | 93cee34fb006c1fec1f907f563f1bde1 | 57b4ede95f6ea09bac2efcbe921fbee07fccf1c7f6b93a0c3ead58d01dd9c020 |
|  1.6.7  | 656e5cb41674a7cb3d0429a87c47da5a | fbd7757f8ff344eb9bf2d9f6c7a01f93281921d818c402b62fb5204059d4c6db |
|  1.6.6  | b7743e84040df7d5bef6f141621eaf9d | 44172fa9d715a35abf9dd4cad22031e20b5f2ac4514ba56d07e7ced11f75522b |
|  1.6.5  | 65b6a3472335b71b3818bbe2d35a706b | b281d49fd4a0c40e62af58960554414627788e858ab716ada242ec028fd95d0a |
|  1.6.4  | f1d22c3f3c5f7c567727a54ae7d68eae | 4c0f0ee20a96f1f4594fc8defbbd7d68ecb1d13080b627e3daf3b233b87baa97 |
|  1.6.3  | 1c0dd378f9fa6cd4e3c645380ae314b9 | 3147424a71f6df65f63c3e92564cf7d55e8b748c79546d929a2938fe47ffdcb7 |
|  1.6.2  | 593210fc806f37fc9e6b979909414d52 | 77063b71a05c12b0d3328ae983417f8b27fe3d2f038a03e0a098266a31659651 |
|  1.6.1  | 2b5c73f176a895135dbfb6ab9337eabb | d959026cc4442dac8f835701c48fe75d029edd5ed9b94b8740f2022c3b8b6eda |
|  1.6.0  | 4985a5d4a8a45f98ccfdf1d039ecf926 | 761cb44ca6be823e11b6e0301fa818aa7fbb4d8b277e8c8e6ba1f7dfe0cf2ae0 |
|  1.5.9  | f4c74ec4d08e26c53ccbcfcdb20c35b3 | cc7daf17bd4a8ac52ee00f1eec49f87a4f081568b42c56280318b804ac744971 |
|  1.5.8  | 4903a5900f0e55daa2bcbb1d5207f4d0 | dfbfcf2ad563fc6aaec87380732bea159f6cf648b13f9397218fd3694b7744e3 |
|  1.5.7  | 343daaecd1618922b9ef9c2811ce61d7 | 24d46dd0a2e899b5ec047ba860375f5d07ff9d4ecc75e914d34f8a423d2af143 |
|  1.5.6  | b90aca7a51d0b01d21530d987ed5d564 | 1861aa2a7afdc5430f2517e9286a65ccbd1a8de42e9d6596b687ae8aa4b43da3 |
|  1.5.5  | 0e2668727560344978dd523925a75a4b | 76bc787cd5933f6f2cd40b7cc227038995c7717985ebaf9031fa61154b0f6360 |
|  1.5.4  | f510204c4fa7533b05e729b902ebec59 | 84e5382013fd5625d684d02836f001d126c31196635e5b1630bc36710ef7afe7 |
|  1.5.3  | 4ebc793117ce677fb07602e31256e7cc | 4b35d2b8237b9708b12d1386527b3a6c233a641a989f7c63b9512cdc522af219 |
|  1.5.2  | 10e6f64debae79bf1e40bd830c6a819e | f357cf564293ad09026170949e7b69e13342b47e57880200b6575c0e596c4e99 |
|  1.5.1  | c30cbf152acc15c5cffafaf7a7a387ad | f1eb4e4571c9c1e08771ffcd896c6aaab63097e2ddda0d00232754d114dc9313 |
|  1.5.0  | aed562118bd5d8c64578f3b52a7b2460 | cf2e8aa6a324f2059b5ec5035ed7fbe27f2ea2d2c7f3792672a803900aa2e37c |
|  1.4.9  | bbe46949fcc243ad113c45ec19ce9215 | d8f605a142c6140905cf25a829f0be10d402e232ce1717013553aaec443d6946 |
|  1.4.8  | 5c5cb0676c72c8d554091ad5a7608471 | 5dedd0c8c793c5f22a3d8d4703e31a6fc5e8d483159b31a1fe64265eefc1f7c3 |
|  1.4.7  | 618c2017ce7f9f75bbdfe09ae06a4467 | 02182af2d93d3c3d63985986c2a0b8c9506223abe15a59278caf67e84f2efece |

### <mark style="color:blue;">The online tools to verify MD5 and SHA256</mark>

There are many tools for online verification of MD5\SHA256 value, and their usage is similar. You only need to drag or load the apk file downloaded to the PC into the verification platform to wait for the result. The obtained result can be verified by comparing it with the MD5 or SHA256 value of the genuine APP published on the official website of TokenPocket<mark style="color:red;">(There may be advertisements and other content in the online tool page, please use the main verification function, and do not recommend anything else).</mark>

Tool 1: Open the link [<mark style="color:blue;">**https://www.dute.org/file-hash-validator**</mark>](https://emn178.github.io/online-tools/sha256\_checksum.html) to select the hash algorithm, usually MD5 is widely used, and the safest algorithm is SHA256. You can also try other hash algorithms. After selecting or dragging the downloaded APK file at the top, the result will be quickly obtained at the bottom. You only need to copy the result and compare it with the officially announced MD5 or SHA256 hash value to complete the verification.

![](../../.gitbook/assets/在线英文1.png)

Tool 2: Open the link http://www.metools.info/code/c92.html, select the file and hash algorithm, click “Calculate”, and you can view the result in the “result”.

![](../../.gitbook/assets/在线英文2.png)

### <mark style="color:blue;">**Tools to verify MD5 and SHA256 on PC**</mark>

MD5 tool:&#x20;

Open the official website of the tool [https://www.winmd5.com/](https://www.winmd5.com/,), Click “Download” to download and open it.&#x20;

{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-MMF2k4MCaxErpZyah2d%2Fuploads%2FKlS0H63nWrUIDmfdtZwN%2FSnipaste_2022-06-20_21-24-51.png?alt=media&token=3d63d392-ff6c-44df-9fa7-536a3a1d9c19" %}

This tool can only verify the MD5 value. Click “browse” to select the downloaded APK file. After importing, you can see the MD5 value prompted below.

{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-MMF2k4MCaxErpZyah2d%2Fuploads%2F6gmzqzprrTYSWsRIgCth%2FSnipaste_2022-06-20_21-31-00.png?alt=media&token=ba4040c8-a3bd-4354-b825-1d0f708a0cd5" %}

SHA256 tool:&#x20;

This tool is our familiar compression/decompression tool 7-Zip, through which you can easily get the SHA256 value of the file.

Open the official website [<mark style="color:blue;">**https://www.7-zip.org/**</mark>](https://www.7-zip.org/) **a**nd click “Download” to download the corresponding version and install it.

{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-MMF2k4MCaxErpZyah2d%2Fuploads%2FocJZCuQGvkYBRdBjTr2H%2FSnipaste_2022-06-20_21-29-07.png?alt=media&token=3108a86d-bd98-4f23-b8ce-5c1486394f2c" %}

After installation, just right-click on the downloaded APK file and select “7-Zip”—"CRC SHA”—"SHA-256” to see the SHA256 hash value.

**Tool :**Click to [<mark style="color:blue;">**download the tool**</mark>](https://cr5.198254.com/com.hobbyone.hashdroid.apk)**.** This tool is more powerful and supports multiple hash algorithm verifications such as MD5 and SHA256. After the same installation, click to switch to “HASH A FILE”, and tick “Select a hash function” to choose, next press “CLICK HERE TO SELECT THE FILE TO HASH” to find the apk that needs to be verified, then click “CALCULATE” after loading. The result can be compared with the official parameters.

{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-MMF2k4MCaxErpZyah2d%2Fuploads%2FBq7gJnSwv9Nz5ZqWyMez%2F2.png?alt=media&token=02354ca7-d56d-4c61-8ec0-5119565ec5f3" %}
