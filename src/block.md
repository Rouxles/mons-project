# Block

Each *block* in a [blockchain](/blockchain.html) records a large number of transactions that have taken place (for example, in Bitcoin it's around 2400)

At the end of each block, there needs to be a 'proof of work' where each result in a block is chained together, and 'miners' find a value that returns a hash that has a set number of 0s at the beginning (which can be changed depending on number of miners)

Each block must contain the hash of the previous block in the header - making a chain. Thus, if you want to change an earlier block, you need to calculate the proof of work for all subsequent blocks too. And at that point, you are simply racing against other miners (assuming proof of work is used instead of proof of stake [links added later!]) - if you have less than 50% of the share of resources in terms of mining, then you won't be able to keep up (in terms of trying to fake data)

The first block in the chain (without any data in the 'previous block hash' field) is called the genesis block.

Whenever the miner gets the correct nonce to make the block data + nonce lower than the target value, the block now is successful and is added to the blockchain. Through this, the miners then get paid a share of the cryptocurrency for their work (which is why miners have an incentive to mine, and a partial reason as to why the mining pool constantly grows)

---

A block is formed by different miners.

When a transaction is made within a cryptocurrency, it doesn't go to the blockchain straight away, but is held in a transaction pool (place where multiple transactions are stored)

A miner aims to gather transactions from the transaction pool into a "candidate block", and then attempt to add this block to the blockchain.

- Each candidate block has a header, which contain the following metadata (data that describes data) about the block:
    - Version: Describes the structure of the data inside the block - this allows miners to know what standard the block is in
    - Last Block: An identification number for the previous block - this is hashed
    - Transactions: This is basically the [**Merkle Root**](/merkle-root.html) where all transactions are hashed into a single string.
    - Time: The current time (when the block was made)
    - Target: This is calculated from the difficulty value which is set by the cryptocurrency network in order to regulate how hard it is to add a block of transactions to the blockchain. Then, the miners will keep hashing the block header with a *nonce* at the start (arbitrary number) in order to get the hash below the target value.

Once a nonce is found that makes the block header + nonce below the target value, the block is solved, and then all transactions of the block are added to the blockchain. The nonce can only be found through brute force, as it has an NP time complexity.