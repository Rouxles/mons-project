# Key Terms and Definitions

## 51% Attack

Definition: When a person or affiliated group of people have 51% or more of the resources in the mining pool in a cryptographic system that uses proof-of-work, allowing them to manipulate the network to their own liking.

Explain: When a block is considered 'valid' on the blockchain, that fork of the blockchain needs to be the longest chain, meaning that in order to create a fraudulent block, you would need to make blocks faster than the rest of the mining pool to get your fork of the blockchain 'trusted', which requires more than 51% of the share of the mining pool and enough luck.

## Block

Definition: A group of a fixed size of transactions from the transaction pool to be inserted into the blockchain. 

> To expand, you could say that each block has a header which contains the previous block hash, the nonce, the version that the cryptocurrency is running on in that block (so other miners know how to read it and what to do with that data), and the hash of the block.

## Blockchain

Definition: A blockchain is made up of several blocks linked to each other by using the hash of the previous block and hash of the current block such that if a single value in one of the blocks is changed, the hash changes, and thus, the chain is 'broken' and is therefore an invalid chain unless all subsequent blocks are re-validated. 

## Candidate Block

Definition: A candidate block is a block to be entered into the blockchain. This is essentially a list of transactions where the nonce hasn't been found to make the hash of the block and the nonce under a certain target value.

## Collision Resistance

Definition: A property of a cryptographic hash function where a function is considered collision resistant if it is very hard to find two inputs that map to the same output.

## Cryptocurrency

Definition: A form of digital currency that is not regulated by a central authority.

## Cryptographic Hash

Definition: A one-way function where an input maps to a unique output of fixed length and where a small change to the input creates a completely different end hash.

## Determinism

Definition: A function is deterministic if one input always maps to the same output.

## Digital Signature

Definition: The use of the transaction data and a private key to create a signature that is attached to each transaction. To verify that a signature is valid, the private key (unique to each person), transaction data as well as the digital signature itself is used together to show whether block funds are linked to the correct person or not.

## Distributed Consensus

Definition: A distributed consensus ensures the consensus of the validity of the data among different nodes in the distributed system (in this case the MONS project). The members of a cryptocurrency are part of a distributed system, and they have to ensure that their individual copies of the blockchain in sync with everyone else's. Each ‘full node’ in the system contains a copy of all the transactions, otherwise known as blockchain. Each block on the blockchain contains transaction history, and when a node adds a transaction or a block to the blockchain, it sends out the information to the rest of the network. The blocks are then validated by the miners and proof of work. If someone is receiving two different blockchains, they will always disregard the shorter of the two chains.

## Double-spend problem

Definition: When the same amount of cryptocurrency is spent in two different places. This is avoided by essentially using the longest block (and this depends on which transaction ends up in the longest block because they're broadcasted to different nodes).

Also linked to why in Bitcoin, you would want your transaction to be 3 blocks deep before feeling safe about it being confirmed.

## Entropy

Definition: Measure of uncertainty associated with a random number generator (also something to do with atmospheric noise/humidity levels/gyroscope sensor type stuff with RNG)

## Genesis Block

Definition: A block without a previous block hash attached to it in the header (effectively the start of the blockchain)

## Immutable Transactions

Definition: Once a transaction is around 3 blocks deep in a blockchain, it is essentially "immutable", which means that the value of that transaction cannot change

(Links to hashing and block headers)

## Key Pair Generation

Public + Private Key generation: RSA Encryption

## Ledger

Definition: A public record-keeping system of all the transactions that have occurred in a blockchain that every full node in the blockchain keeps a copy of.

## Merkle Proof + Merkle Tree

Definition: A method to get all the transactions hashed in a block (by essentially using a binary tree structure to make a final hash)

This takes off some computational workload when used.

## Miner

Definition: A node that works to put transactions in a candidate block and find a nonce that makes the hash go below the target value to then be placed on the blockchain. They get a bit of reward in BTC for doing this.

## Mining

Definition: Finding a nonce that makes the block hash + the nonce hashed together below a certain target value 

## Nonce

Definition: Number only used once - hashed together with a block to hopefully get something to be below a target value for that thing to be a 'valid' block.

## Non-invertibility

Definition: Goes hand in hand with a one-way function and is important for hashing functions (can only go one way, very hard to go the other way)

## Non-repudiation

Definition: A situation where it is impossible to deny the authorship of a digital signature. In essence, message senders are unable to falsely claim that they did not send the message.

## One-way function

See above [Non-invertibility](#non-invertibility)

## Proof of work

A paradigm in cryptocurrency used where people find a nonce below a certain target value (aka mine the block) to make sure that it is valid.

## PuTTYgen

PuTTYgen is a software used to generate public and private SSH keys (RSA keys being one of them).

## Self-referential Data Structure

Points to the same kind of structure (ie singly linked list)

## SHA256

Definition: Is a hashing algorithm

## Takeover Attack

Definition: 

## Transaction Pool

Definition: 'Waiting area' for all transactions that each full node has for themselves.