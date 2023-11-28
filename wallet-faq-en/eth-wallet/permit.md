# What is Permit

Permit is an optimization proposal introduced in EIP-2612 to enhance the interaction mechanism for ERC-20 standard tokens. When using the Approve token authorization under the ERC-20 standard, users are required to pay ETH as gas fees. With the Permit method, users can generate a signature offline using their private key for authorization. The entity possessing this signature, such as a smart contract, can then directly invoke the Permit function to facilitate token transfers without requiring users to pay gas fees for Approve authorization.

The method enabled by the EIP-2612 extension for ERC-20 is typically as follows:

<figure><img src="https://511045620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F3qtItoZih7cEdFc6kPNk%2Fuploads%2FzkCZqtUGyzXzb204uZxr%2Fimage.png?alt=media&#x26;token=c74a98c1-9bae-4d57-ad32-79d0d44fae0c" alt=""><figcaption></figcaption></figure>

1. Alice signs an off-chain "permit (signature authorization)" message, indicating her desire to grant a contract permission to use a token under the (EIP-2612) standard.
2. Alice submits the signed message as part of her interaction with the contract.
3. The contract calls the "permit()" method on the token, using the signed authorization information and signature, thereby granting the contract permission.
4. With the authorization in place, the contract can now call transferFrom() on the token to transfer tokens held by Alice.&#x20;

Since Permit (EIP-2612) requires the relevant methods to be implemented within the ERC20Token contract, previously deployed ERC20 contracts cannot support it. (In other words, it is more suitable for newly issued tokens.)

This addresses two issues with the typical ERC20 approval methods:

1. Users are not required to additionally submit an on-chain approve() interaction.
2. By eliminating one on-chain operation, users can generally choose a more reasonable approval amount, rather than an unlimited allowance. Moreover, it is crucial that an expiration time can be set when signing the authorization message.
