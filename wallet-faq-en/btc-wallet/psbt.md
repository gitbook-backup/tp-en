# What is a Partially Signed Bitcoin Transaction (PSBT)

Bitcoin PSBT (Partially Signed Bitcoin Transaction) is a transaction description format used for constructing and processing Bitcoin transactions. It provides a secure and flexible way for multiple participants to collaborate in building and signing Bitcoin transactions without exposing private keys.

PSBT is a data structure that includes transaction information and partial signature data. Its main purpose is to allow participants to exchange transaction data while performing partial signatures to complete the process of building a Bitcoin transaction. Since different participants may have different private keys, they can add their respective partial signature information to the PSBT according to specific protocol rules.

The design of PSBT is highly flexible and can adapt to various use cases. Here are some common use cases:

**Multisignature transactions:** In multisignature transactions, multiple participants' signatures are required to complete the transaction. With PSBT, each participant can individually perform partial signatures on the transaction and then combine them into a complete transaction. This method provides higher security because private keys are not transmitted between participants.

**Hardware wallets:** Hardware wallets typically store private keys in secure physical devices to provide enhanced security. With PSBT, a hardware wallet can perform partial signatures internally and return the signature data to the connected computer. This way, the private keys do not leave the hardware device, offering better protection.

**Advanced transaction construction:** Some Bitcoin transactions may have complex construction requirements, such as multiple inputs and outputs, multiple script types, etc. With PSBT, participants can gradually build the transaction and add necessary partial signature information at each step. This makes it more flexible and controllable to construct and adjust complex transactions.

It's worth noting that PSBT is only a transaction description format and not part of the core Bitcoin protocol. Therefore, not all Bitcoin nodes directly support PSBT. However, many popular Bitcoin wallets and tools have already embraced PSBT, making it convenient to use PSBT for constructing and processing Bitcoin transactions on these platforms.
