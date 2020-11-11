# November 2020 Paper 3 Past Paper

> These notes aren't too good right now - these will be changed.

1a - Identify 2 characteristics of Peer-to-peer network [2]
- A peer to peer network contains multiple nodes connected to each other, where each node acts as both a client (receiving data) and a server (sending data).
- Scalable
- Seeding - can be used to say how reliable one connection is over another connection. (Sort of like a trust mechanism)

1b - Identify 2 sources of entropy. [2]
- Atmospheric Noise - True RNG
- Time - Pseudo RNG
- Light level in the atmosphere
- Temperature/Humidity

---
  
2a - Describe the steps that need to be carried out by the blockchain system to find a user's central MONS balance [4]
- The blockchain system calculates the balance of each user by looking at the transaction history. 
- When a user needs their balance calculated (for future transactions for example), each node looks at transactions associated with the user (both as the sender and the receiver), and then calculates how much cryptocurrency has been given to the user, and how much cryptocurrency the user has given away to other users.
- These two values are then added up together (with the cryptocurrency the user given away being negative) to find a user's MONS balance.
- UTXO - sequentially goes through UTXO for each user from the start of the block to the end of the block.
- The block when split - calculations are done that way
- Blocks have to be validated in order for the transaction to be valid.

Dolores states "one of the great things about the blockchain is that we can ensure that the solution time remains at 10 minutes, and we can do this even as the number of MONS miners increases" (lines 63-65).

2b - Explain why it is important to ensure the solution time remains at 10 minutes. [4]
- By setting the solution time at 10 minutes, a block can only be added to the blockchain every 10 minutes.
- Making the solution time take 10 minutes (as opposed to 2 seconds) allows more transactions from the memory pool to be placed in a blockchain, and also helps with making sure transactions are non-malicious. As the solution time is 10 minutes, if a malicious user decides to edit transactions 3 blocks down, they would need to spend 30 minutes to find correct nonces to keep the blocks chained to each other. By the time they finish finding correct nonces, other miners would have added blocks to the blockchain, leading to 30 minutes of wasted time by the malicious users.
- Also to ensure that the difficulty of mining the block does not change as the currency gets more popular.

---



