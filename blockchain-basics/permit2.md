# What is Permit2

### <mark style="color:orange;">About Permit2</mark> <a href="#about" id="about"></a>

Uniswap has just released a new token approval standard, Permit2, which differs from the traditional ERC20 and EIP-2612. Permit2 allows users to avoid the need for a chain-level “approve” operation before interacting with different DApps, allowing the DApp protocol to first acquire your token approval. According to the description, the new Permit2 protocol has the advantages of saving gas, allowing for batch operations of approval/transfers and being more flexible than traditional ERC20 approval, and supporting one-stop approval management.

Uniswap initially conceived Permit2 and Universal Router to improve its own product, optimize gas costs, simplify the user transaction process, and enhance security. During the conceptual process, Uniswap felt that other applications could greatly benefit from integrating these contracts. Uniswap itself is dedicated to building public infrastructure, so it designed these contracts to be available for use by the entire developer ecosystem, including extensive documentation and SDKs.

To illustrate how revolutionary Permit2 is, let’s review the previous solutions by taking the example of a contract that needs to move tokens held by Alice.

### <mark style="color:orange;">Traditional approval model</mark> <a href="#tradition" id="tradition"></a>

The traditional way of execution is shown in the following diagram.

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FZCSGxZxDUFXGuknjRHbB%2Fuploads%2F9APh5PNStCAlcssu4SUg%2Fimage.png?alt=media&#x26;token=ee47c2b4-91d1-42a0-aa6b-a2b3cfadcf40" alt=""><figcaption></figcaption></figure>

1. Alice calls the approve() function on the ERC20 to grant the contract a controlling limit.
2. Alice calls an interaction function on the contract, which in turn calls transferFrom() on the ERC20 token contract to move her tokens. It is evident that this model is feasible (as it is widely existent) and can ultimately be very flexible, as the protocol can continually access the user’s tokens for an extended period of time.

**The approval contract is granted the approval to control the maximum amount of tokens by default, without any time limitations. Each DApp requires a one-time approval for the first execution, which poses significant risks.**

But it faces two well-known real-world problems:

1. Poor user experience: Users must grant approval for each new protocol they intend to use on each token, which is almost always a separate transaction (for example, executing a token approval in Uniswap, but still having to reapprove if using Transit).
2. Poor security: Contracts usually require an unlimited approval limit, and approval must be executed every time a swap or other contract is used. This means that if the protocol is exploited, every user who has approved the protocol to consume their tokens could have all of their approved tokens transferred. (For example, we often encounter token usage approval, such as approval to operate DeFi, approval to exchange, and approval for first-time use of different DApps)

### <mark style="color:orange;">Permit (EIP-2612) mode</mark> <a href="#eip2612" id="eip2612"></a>

EIP-2612 iterates on token approval. Users can interact with the application contract by attaching an approval signature (Permit) information in their transaction, without having to pre-approve.

Let’s take a look at the methods enabled by the EIP-2612 extension of ERC20, which is usually like this:

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FZCSGxZxDUFXGuknjRHbB%2Fuploads%2FqsueYCqpcNIuIIboOFlp%2Fimage.png?alt=media&#x26;token=49f43286-484d-4c87-8a88-8bb032863eaa" alt=""><figcaption></figcaption></figure>

1. Alice signs a “permit” message off-chain, indicating that she wishes to grant a contract the right to use an (EIP-2612) token.
2. Alice submits the signed message as part of her interaction with the said contract.
3. The contract calls the “permit()” method on the token, which uses the signature approval information and signature to grant the contract permission.
4. The contract now has permission, so it can call transferFrom() on the token, transferring tokens held by Alice.

**Due to the requirement of EIP-2612 (Permit) to have the related methods written inside the ERC20 token contract, existing deployed ERC20 contracts cannot be supported.**

This resolves two problems with the typical ERC20 approval method:

1. The user does not need to submit an additional approve() transaction on-chain.
2. &#x20;Since one on-chain operation is omitted, a typically more reasonable approval amount can be chosen instead of unlimited, and more importantly, an expiration time can be set when signing the approval message.

While EIP-2612 makes token approval more secure, tokens released before EIP-2612 do not support signature approval and not all newer tokens have adopted this feature. Therefore, the protocol is not widely used.

### <mark style="color:orange;">Permit2 Approval Model</mark> <a href="#approve" id="approve"></a>

Permit2 combines both models, extending the user experience and security advantages of EIP-2612 to also cover standard ERC20 tokens.

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FZCSGxZxDUFXGuknjRHbB%2Fuploads%2FVmfM9ezm3LlxGsp120JK%2Fimage.png?alt=media&#x26;token=217e3616-fd01-4baa-8243-5b43e6417ece" alt=""><figcaption></figcaption></figure>

1. Alice calls approve() on an ERC20, in a typical way, giving Permit2 contract limitless approval.
2. Alice signs a Permit2 message off-chain, indicating that the protocol contract is allowed to transfer tokens on her behalf.
3. Alice calls an interaction function on the protocol contract, passing in the signed Permit2 message as an argument.
4. The protocol contract calls permitTransferFrom() on the Permit2 contract, and Permit2 contract uses its approval (granted in 1) to call "transferFrom()" on the ERC20 contract, transferring tokens held by Alice.

By granting approval to Permit2, DApps that use the Permit2 protocol only need to perform a 712 local signature once, eliminating the need for additional chain-level approval and reducing Gas fees, while increasing usability and security. The approval is time-limited, for example, if granted for a month, then after the month expires, it only requires one 712 signature to be used again.By granting approval to Permit2, DApps that use the Permit2 protocol only need to perform a 712 local signature once, eliminating the need for additional chain-level approval and reducing Gas fees, while increasing usability and security. The approval is time-limited, for example, if granted for a month, then after the month expires, it only requires one 712 signature to be used again.

The protocol will not directly call the transferFrom() on the ERC20 token to execute the transfer but instead will call the standard Permit2 contract's permitTransferFrom(). Permit2 sits between the protocol and the ERC20 token, tracking and validating the permit2 message, and then ultimately using its approval to execute the transferFrom directly () call on the ERC20. This indirectness allows Permit2 to extend the benefits similar to EIP-2612 to every existing ERC20 token.

### <mark style="color:orange;">Advantages of the Permit2 protocol:</mark> <a href="#advantages" id="advantages"></a>

1. Unified token management
2. Controllable approval time
3. No need to send a transaction for approval every time

### <mark style="color:orange;">Possible Risks of Permit2</mark> <a href="#risk" id="risk"></a>

Permit2 is derived from EIP 2612 and is an extension of the EIP 20 protocol, so ultimately, Permit2 is just a supplement to ERC20, not a replacement. After all, Permit2 doesn't inherit all existing ERC20 data, and the so-called one-stop management still requires calling the approve function of the ERC20 contract to complete some initial operations.

**The complete process of Permit2 should be:**

1\. The user grants the maximum approval of ERC20 tokens to the Permit2 contract.

2\. The user manages specific approvals through the permit function in the Permit2 contract.

3\. Third-party protocols and users can transfer tokens through the Permit2 contract as an intermediary based on the approval information already available in Permit2.

### <mark style="color:orange;">Possible risks of the Permit2 protocol:</mark> <a href="#risks" id="risks"></a>

1. Although it claims to solve the infinity approval problem, it only transfers the approval object from the interacting DApp to the Permit2 contract, and the security of the Permit2 contract requires higher standards for centralized management of approvals.
2. Although the token approval has an expiration time, this time can still be unlimited, and Dapps still need to set reasonable expiration times.
3. Because the permit function call process can be performed without sending a transaction, just providing a signature to a third party for forwarding, it can be more concealed if it is used for phishing. The cost of checking the signature message increases, and some third-party wallets may not decode and display the signature information, increasing the risk of user attack.

**Advantages and risks exist at the same time, which requires us to have a certain discernment ability. Specifically, the wallet also needs to have prior prevention for the possible large-scale support of Permit2 in the future (TokenPocket does not yet support the parsing of Permit2, but will soon). For example, TokenPocket's current approval risk warning pop-up windows can display the risk content well, thus avoiding risks such as phishing or malicious approval from third parties.**

**Do not open unknown websites and execute them recklessly. Be sure to use regular DApps and control the amount of tokens granted to contracts as much as possible. Regularly use authorization check tools for inspection.**
