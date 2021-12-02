# Venus User Guide (BSC)

**About Venus:**&#x20;

Venus is a complete algorithmic cryptocurrency marketplace protocol running on the Binance Smart chain (BSC), designed to provide platform users with a decentralized and secure marketplace to access loans, earn interest and mint synthetic stablecoin VAI. the protocol design is based on the architecture and fork of Compound and MarkerDAO and is synchronized to the Venus platform, combining the two systems’ advantages.

**About XVS:**&#x20;

XVS is the platform's native BEP-20 governance token, which is primarily used to participate in platform governance, such as voting on product upgrades, adding new collateral types, adjusting platform parameters, etc. XVS is issued through a fair launch mechanism, with no founder or team allocation, and is backed by a well-funded organization and Swipe's team. 20% of XVS's total $30 million is allocated to the Binance launch pool project, 1% to the Binance smart chain ecosystem, and the remaining 79% all based on liquidity mining, with 35% of the daily rewards allocated to borrowers, 35% to depositors and 30% to stablecoin minting users.



**Tutorial:**&#x20;

1: Launching Click the【Discover】in TokenPocket Wallet (BSC) and type Venus on the top of search bar to launch it.

![](https://tp-statics.tokenpocket.pro/token/tokenpocket-1619159986805.png)



2: Deposit The first thing you see when you open it is the number of XVS and VAI I have, and the yellow section is my borrowable amount. Down the page you can see some data on the lending market, such as currency prices, number of deposits, total amount borrowed, annualized lending, etc. You can click to select the currency market information you want to view.

![](https://tp-statics.tokenpocket.pro/token/tokenpocket-1619160068089.png)

You can make a deposit in the 【Supply Market】 section and see the APY for each currency. Here I chose to deposit USDT and can see that the current APY for USDT deposits is 5.02% and the APY for XVS mining is 6.13%. The first time you deposit, you need to click 【Enable】 to authorize, you need to pay a small amount of BNB gas fee, then enter the amount and click【Supply】 to deposit successfully.

![](https://tp-statics.tokenpocket.pro/token/tokenpocket-1619160125563.png)

After a successful deposit your balance and interest APY will be displayed. When you turn on the button at the top of the page, it shows the interest plus mining’s APY. When you turn off the button, it only shows the APY from interest.

![](https://tp-statics.tokenpocket.pro/token/tokenpocket-1619160163826.png)



3: Loan The loan starts with a deposit and requires users to turn on the 【Collateral】button to do next step. When the deposit is enabled, vTokens credentials are obtained, which can be used to lend or issue stablecoins. The maximum loan amount available for deposits is 1:0.6. For example, a deposit of 10U in a deposit currency can be loaned up to 6U in any other currency. Firstly, click the button and use USDT as collateral, then click the 【Borrow Market】section to make a loan, you can see the loan interest rate and the number of liquidity pools for each currency, here I have chosen to loan USDC as an example.

![](https://tp-statics.tokenpocket.pro/token/tokenpocket-1619160210703.png)

Click on ‘SAFE MAX’ and the system will automatically enter the maximum number of safe loans, the general ratio is 1:0.25, I deposited 50U, so the safe number here is 12, of course, we can enter the number of loans more or less than the safe value, but the maximum will not exceed 50 \* 0.6U = 30U. I entered 30 here, you can see that my loan amount has reached 99.9% maximum.

![](https://tp-statics.tokenpocket.pro/token/tokenpocket-1619160249741.png)

The higher the number of loans, the less secure it is and the more likely it is to be liquidated.

Liquidation: A user's collateral may be liquidated if it falls below the threshold required for borrowing or stablecoin in a particular currency market. These liquidations entail payment of liquidation fees and repayment of outstanding debts, with the remaining collateral (if any) then reverting to the user. The main risk of liquidation arises from the total value of collateral assets and the total value of loan assets, the higher the risk of being liquidated when the total value of pledges falls (falling prices of collateral currencies) or the total value of loans increases (rising prices of loan currencies). **Liquidation risk can be reduced by increasing collateral or by early partial repayment.**



**4: Repayment**&#x20;

Open【Repay Borrow】 to make repayments. To make your first repayment, click on【Enable】 to authorize, then enter the amount to be repaid and the interest rate, and click on 【Repay】

![](https://tp-statics.tokenpocket.pro/token/tokenpocket-1619160440996.png)

****

**5: Stake and Mint Stablecoin VAI**&#x20;

The Venus protocol allows users to use v-tokens of the underlying collateral they previously provided to the protocol to mint and issue of VAI, which is a 1:1 on-chain pledge-based stablecoin anchored to USD. The concept that users can pledge assets in the Venus protocol to generate USDE is similar to a home mortgage. In this analogy, Venus is like a bank, the assets staked by users are like a property, and the VAI generated is like the fiat currency that the user loans away, which can be used to make loans and swap for other currencies.&#x20;

Users issue VAI by staking deposits and also receive XVS rewards.&#x20;

First open【Mint/Repay VAI】 in the lending market and enter the number of VAI to be minted, there is also a safe value and a maximum value to be minted, same as the loan amount above, my previous deposit voucher was 50U, so the default safe value is 12U and the maximum can be minted is 30U. Minting is done for a small BNB gas fee.

![](https://tp-statics.tokenpocket.pro/token/tokenpocket-1619160513863.png)

The minting of VAI creates debt and is also subject to the risk of liquidation, mainly through a fall in the total value of collateral assets or an appreciation in the total value of the VAIs issued, which can be mitigated by increasing the collateral or repaying part of the VAI.



**6: Repay VAI**&#x20;

Click on Repay at the bottom of the page to make repayments. You will need to authorise your first repayment, then enter the number of VAI to be repaid and click on 【Repey VAI】 to make the repayment. Once the VAI has been repaid, you will receive the appropriate amount of credit.

![](https://tp-statics.tokenpocket.pro/token/tokenpocket-1619160779142.png)



**7: Voting**&#x20;

Venus is designed for community autonomy, with no pre-determination by the team, developers or founders, the protocol will be executed by the proposal of those holding XVS tokens. Users holding XVS will receive votes corresponding to them, and these votes can be allocated to themselves, or they can fill in someone else's address to have someone else vote by proxy.



**8: Collect Mining Rewards**&#x20;

Click 【Vote】 on the top right of page, you can see your XVS token balance, XVS earnings from borrow mining and from minting VAI. Use【Collect】 button to get XVS rewards.

![](https://tp-statics.tokenpocket.pro/token/tokenpocket-1619162118927.png)



You can see your 【Voting Weight】 at the bottom of the page, click on 【Get Started】to vote, there are 2 modes of voting: Mannual Voting is to vote for your own proposal; Delegate Voting is to let someone else vote by proxy, you only need to fill in the address of another person, no XVS transfer is involved.&#x20;

**Proposal:** You can create your own proposal by clicking on **\[**Create Proposal**]**. Proposers need to have at least 300,000 XVS and the proposal must have a minimum of 600,000 XVS to be approved.

__

_This tutorial is only for the DApp in the wallet side of the operation guide, does not represent the investment advice of TokenPocket. Investing involves risks, you should be fully aware of the risks and make your own investment decisions._

![Scan the QR Code to download TokenPocket](https://tp-statics.tokenpocket.pro/dapp/tokenpocket-1615532554741.jpg)
