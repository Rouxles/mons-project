# Mindmaps

This will contain a collection of 'mindmaps' in a list form based around different parts of cryptocurrency. These can be used for revision purposes.

---

## Blocks

### Header

- This contains metadata - information about the (information of the) block.
  - Version
    - Describes the 'standard' of the block - miners can know what structure the data is in and the conventions that the version is associated with.
  - Last Block (Previous Block Hash)
    - Identification number for the previous block.
  - Transactions (Merkle Root)
    - All the transactions are hashed into a single string using the Merkle Root.
  - Time
    - The current time of when the block was created.
  - Target ([Nonce](#nonce))
    - This is calculated by the 'difficulty value' set by the cryptocurrency network to regulate how hard it is to add a block to the network. (Basically people need to keep incrementing the [nonce](#nonce) (alongside the hash data) until the value of the hash is below the target value - related to [hashing](#hashing))
  - Nonce
    - This is a value that people can use to verify

### Genesis Block

- This [block](/block.html) is one without a value in the header for the previous block
  - This means that the block is the first in the [blockchain](#blockchain) (the one that starts the chain)

### Blockchain

- The blockchain is basically many blocks linked together. In the [header](#header) for each block, they're linked to the hash of the previous block. The validity of the chain is dependent on the previous block being integral, meaning that if you wanted to change a transaction in one block in the chain, you would need to find the correct [nonce](#nonce) for all the previous blocks beforehand faster than the rest of the mining pool.
- 

<!--List of transactions and header-->

---

## Security

### Hashing

#### Nonce

### Digital Signatures

---

## Mining

### Mining Pool

### 51% Attack

This happens when a single party has more than 51% of the share of the mining pool.

---

## Transactions