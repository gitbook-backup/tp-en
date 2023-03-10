# About self-custodial staking

Self-custody staking is a way to participate in validating transactions on the Ethereum 2.0 network by holding at least 32 ETH and running a node. However, for ordinary users, there may be some common issues to address:

### <mark style="color:orange;">1.What is self-custody staking?</mark>&#x20;

Self-custody staking refers to the process of holding at least 32 ETH and running a node to participate in validating transactions on the Ethereum 2.0 network. This requires users to have a certain level of technical ability and security awareness to ensure the stability and security of the node. To simplify participation for ordinary users, and to ensure that the funds are under the control of the user, the Ethereum staking roles can be split into stakers and validators, with users holding credentials and permissions related to funds and the node hosting party holding permissions related to node management, to ensure the security, stability, and continuous rewards of the node.

### <mark style="color:orange;">2.What are the withdrawal and signing private keys, and who holds them?</mark>&#x20;

The withdrawal private key is held by the user and is used to withdraw staked funds and validate rewards. The signing private key is held by the node manager and is used for node validation of transactions.

### <mark style="color:orange;">3.What fees are required for self-custody staking?</mark>&#x20;

Participation in self-custody staking requires payment of fees for transaction validation and node operation. In addition, a certain amount of staked funds is required, with each validator required to stake 32 ETH.

### <mark style="color:orange;">4.When can I withdraw my funds, and what is the difference between exiting and withdrawing?</mark>&#x20;

You can indicate your intention to stop validating by signing a voluntary exit message with the validators. However, please note that once you exit, there is no turning back, and you cannot reactivate the validator, nor can you transfer or withdraw your funds until the withdrawal function is enabled. This function is proposed to be included in the next network upgrade (i.e., the "Shanghai Upgrade"). This means that your funds will remain unavailable at least until the Shanghai Upgrade. Shanghai Upgrade：https://ethereum-magicians.org/t/shanghai-core-eip-consideration/10777

### <mark style="color:orange;">5.What are the risks of running a node yourself?</mark>&#x20;

Running a node yourself requires ensuring the stability and security of the node, otherwise you may face risks such as node attacks and staked fund losses. Two important scenarios to note are:

a.Offline in the majority (2/3) of validators will lead to relatively minor penalties because there are still enough validators online to complete the chain. This is expected.

b.Offline when the total number of validators exceeds (1/3) will result in more severe penalties because the block is no longer finalized. This scenario is very extreme and unlikely to occur.

### <mark style="color:orange;">6.What is a withdrawal credential?</mark>&#x20;

The withdrawal credential is a 32-byte field in the deposit used to verify the target address for a valid withdrawal. Currently, there are two types of withdrawals: BLS withdrawals and Ethereum address withdrawals. After the first deposit, you cannot modify your validator withdrawal credentials, so you need to keep your withdrawal private key safe.

### <mark style="color:orange;">7.What happens if my withdrawal private key is stolen?</mark>&#x20;

If your withdrawal private key is leaked or stolen, the thief can transfer your validator balance, but only if the validator has already exited. If the validator signing key is not under the thief's control, the thief cannot exit your validator. Using your signing key, you can try to exit the validator quickly and then transfer the funds using the withdrawal key before the thief does.

### <mark style="color:orange;">8.Is there an annual fee for TokenPocket's self-custody node?</mark>&#x20;

No, there is no annual fee for TokenPocket's user self-custody node. A one-time service fee is charged, and no further fees will be collected thereafter.
