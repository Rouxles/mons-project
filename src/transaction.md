# Transactions

## Coinbase Transaction

This is the transaction that goes to the miner when they successfully mine the block.

When people make transactions, they can put a "fee" on it which they pay. This fee goes to the miner if they successfully mine a block.

This fee is essentially like a priority ticket. The more you pay, the further ahead in the queue you are. This is because miners aim to make the largest amount of profit, so they are going to put a transaction from their [memory pool] to a [candidate block] with the highest reward per bit size.

### Fee per Byte

Every transaction takes up a certain amount of space, and 
