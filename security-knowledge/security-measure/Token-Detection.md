# Token Security Detection Function Use Guide

Token trading through DEX is an often-used function in our daily life. Because of the openness of DEX, any person or team can list different types of tokens. In this process, some criminals will play tricks in the token contract, for example, issue tokens unable to be sold(honeypot) and tokens with additional issuance functions. So, it is necessary to use the token contract security detection tool. Although the detection cannot be guaranteed to be 100% accurate, it can eliminate some risks and allow users to choose safer tokens for transactions.

1、Open TokenPocket, click on any token to be detected, and tap “Project Details” in the upper right corner.

![](<../../.gitbook/assets/1 拷贝 (1) (2).png>)

2、In the details interface, you can see the token information such as contract address and issuance volume. In the lower part, you can see the risk warning of the token, which is generally divided into “Security Warning” and “Danger Warning”, and the latter is most dangerous. Click “View more security information” to jump to the contract detection details, where you can view the security detection details of the token contract address.

![](<../../.gitbook/assets/3 拷贝 (2).png>)

3、At the top of the detection interface is a built-in gadget. Click the icon on the left to select the public chain supported by the tool, currently supporting Ethereum, BSC, Polygon, Avalanche, Arbitrum, Heco, OKC, Fantom, Harmony and Cronos, and more chains will be available.

Choose the public chain, fill in the contract address and click “Detect” to conduct the contract detection of the token.

![](<../../.gitbook/assets/5 拷贝.png>)

**4、**Now we have been familiar with the entry and functions of this tool, and next introduce some common “Danger Warnings” and “Security Tips”.

Proxy contract: bind another contract in the token contract code. The contract can control additional issuance, transaction switch and other functions, which is more dangerous.

Honeypot token: can’t be sold, so the token has no value.

Whitelist function: only those who are on the whitelist can buy and sell tokens.

Anti-whale function: Prevent bulk buying to gain control of tokens.

![](<../../.gitbook/assets/7 拷贝.png>)

Blacklist function: Addresses added to the blacklist cannot sell tokens. This setting can be combined with the anti-robot function.

Additional issuance function: Increase the function of token issuance, for example, some mining projects use it for mining or some malicious projects increase issuance to smash.

![](<../../.gitbook/assets/6 拷贝.png>)

The launch of this tool can largely help users to avoid some malicious tokens. It is only for reference, and it cannot be 100% guaranteed to be accurate. Subsequent functions will be added to the token details of the market interface.

The Token Contract Detection Tool can also be used by copying the link to the DApp browser at [<mark style="color:blue;">**https://tokensecurity.tokenpocket.pro/?utm\_source=tokenpocket#/**</mark>](https://tokensecurity.tokenpocket.pro/?utm\_source=tokenpocket#/)<mark style="color:blue;">****</mark>

