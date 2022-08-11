# Phishing wallet scam

Recently, many community members have reported that they encountered errors when transferring money using TRON wallet. After digging deeper, we found that they have something in common. They all obtained a shared private key or mnemonic from the Internet. After importing with the keys, they could see some assets on the TRON wallet, but there was not enough TRX as gas fee. So, they deposited TRX to transfer these assets, but failed. the transfer of any kind of token would report an error. The following will detail the essence of this phishing wallet scams.



1、Use the shared private key or mnemonic to import, select a token such as USDT to transfer when the gas fee is enough, then fill in the receiving address, set the amount, enter the password, finally find a bunch of code error messages pops up.

{% embed url="https://1241502402-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FMr66Ca6n3UR4Xw7gcij2%2Fuploads%2FDJVmjjFI8muIJngGAzZb%2F1.png?alt=media&token=07739146-1093-4cb0-9bd9-e0cbc5ef7a05" %}

2、Click on the receiving address in the picture above, and record it, which will be used later. Open the TRON blockchain browser: [<mark style="color:blue;">**https://tronscan.io/#**</mark>](https://tronscan.io), and type the receiving address for inquiry. In order to demonstrate intuitively, we choose the browser content on the PC to display here.

{% embed url="https://1241502402-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FMr66Ca6n3UR4Xw7gcij2%2Fuploads%2FP2QG9Tj2uuCT5q5Tqy4V%2FSnipaste_2022-07-05_16-25-46.png?alt=media&token=a683b83d-1540-4c0a-a084-2fa161aa4dff" %}

In “Account Permissions”, you can see that both the owner and active permissions are the same addresses, but they are different from the wallet receiving address, which obviously explains why all imported assets cannot be transferred.

Let me give a brief explanation. The TRON public chain integrates some features of Ethereum and EOS, so it has basically the same permission settings as EOS, including owner, active, weight, threshold. For specific function descriptions and operations, please refer to the official multi-signature documentation:\
[<mark style="color:blue;">**https://cn.developers.tron.network/docs/multi-signature**</mark>](https://cn.developers.tron.network/docs/multi-signature)

We would like to remind everyone here that there is no lunch for free. This kind of scam to cheat gas fees is a relatively early one. Users would lose some gas fees at most, but if they encounter scams such as “malicious approval” or “call contract to steal a token”, the loss will be relatively enormous.
