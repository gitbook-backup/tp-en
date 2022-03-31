# Does a bitcoin address have to start with a number?

No, there are 1, 3 and bc1, which represent the following:

The address at the beginning of 1 is P2PKH(pay-to-public-key-hash) address, which is the original address, and is called ordinary BTC address;&#x20;

The address at the beginning of 3 is P2SH(pay-to-script-hash) address, and the internal address also needs to be segwit, that is, the segwit address.&#x20;

The address at the beginning of bc1 is a BECH32 encoded address, an address format developed specifically for segwit, and an segwit address.&#x20;

The address at the beginning of 3 and bc1 are smaller and less expensive than that of 1, which can improve the packaging speed of BTC block.
