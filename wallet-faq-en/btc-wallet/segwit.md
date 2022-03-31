# What's the SegWit

Segregated Witness \(abbreviated as SegWit\) is an implemented protocol upgrade intended to provide protection from transaction malleability and increase block capacity. SegWit separates the _witness_ from the list of inputs. The witness contains data required to check transaction validity but is not required to determine transaction effects.

Additionally, a new _weight_ parameter is defined, and blocks are allowed to have at most 4 million weight units \(WU\). Non-witness and pre-segwit witness bytes weigh 4 WU, but each byte of Segwit witness data only weighs 1 WU, allowing blocks that are larger than 1 MB without a hard forking change.

