# How many bits is the bitcoin address?

The length of a typical BTC address is 26-34 bits. It's worth noting that the address of the bitcoin is not the public key, but the hash of the public key. That is, the address can be derived from the public key, but the public key cannot be deduced from the address, because the hash function is a one-way function.

Tips：

The address at the beginning of 1 is P2PKH\(pay-to-public-key-hash\) address, which is the original address, and is called ordinary BTC address; 

The address at the beginning of 3 is P2SH\(pay-to-script-hash\) address, and the internal address also needs to be segwit, that is, the segwit address. 

The address at the beginning of bc1 is a BECH32 encoded address, an address format developed specifically for segwit, and an segwit address. 

The address at the beginning of 3 and bc1 are smaller and less expensive than that of 1, which can improve the packaging speed of BTC block. 

The BTC address of Satoshi Nakamoto: 1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa

