# Brief Introduction to Cryptocurrency

## Background
In 2009, Satoshi Nakamoto released a paper entitled \textit{Bitcoin: A Peer-to-Peer Electronic Cash System} detailing his vision of commerce.  Nakamoto's vision detailed a peer-to-peer currency system backed by a hash based proof-of-work.  The network would timestamp transactions by hashing them into an ongoing ledger that could not be changed without redoing the proof-of-work.  Nodes would choose the longest chain as proof of events witnessed by the largest pool of hashing power.  As long as $\geq$ 51% of the network hashing power is controlled by nodes not intending to facilitate an attack, the chain they generate will remain the longest. [@Bitcoin]

## The Block
Each block on the network is prefaced with an 80 byte header containing a double SHA256 hashed copy of the previous block's header, merkle root (a double SHA256 hashed derivation of all the hashes that occurred in the block), the time stamp at which proof-of-work began, difficulty target this header's hash must be less-than or equal to, and the nonce at which miners reached the difficulty target.  As such, any attempts to modify any transaction in any block will result in the rejection of the block by the network's miners.  [@Bitcoindev]

## The Blockchain
Groups of transactions are formed into blocks and those blocks are placed chronologically into a chain - forming the blockchain.  The blockchain creates a moving history of all of the activity within the network and serves as a distributed consensus model where any transaction can be verified at any time [@Crosby].  

## Proof-Of-Work
Proof-of-work is a system of verification in which miners must devote tangible resources (electricity, hardware costs) to solve an arbitrary probabilistic \textit{word puzzle}.  In order for a bad actor to taint the blockchain with a fraudulent transaction, they must complete all proof-of-work up to the present point. [@Bitcoindevreference]
