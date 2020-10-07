# Transactions

## Coinbase Transaction (additional information)

This is the transaction that goes to the miner when they successfully mine the block. Think of this as like putting your name on the top of a lottery sheet in order to address the contents of the reward to you.

When people make transactions, they can put a "fee" on it which they pay. This fee goes to the miner if they successfully mine a block.

This fee is essentially like a priority ticket. The more you pay, the further ahead in the queue you are. This is because miners aim to make the largest amount of profit, so they are going to put a transaction from their [memory pool] to a [candidate block] with the highest reward per bit size.

The transaction amount is then checked by other nodes to see if it's calculated correctly. If not - the block reward will not be given to the miner.

Additionally, these coinbase transactions will only be transferred over to the miner once the block is 100 blocks deep (in Bitcoin) to basically ensure that the transaction is not fraudulent.

### Fee per Byte

Every transaction takes up a certain amount of space, and each transaction may take a different amount of space. As a block has a limited size (around 1 MB for a block), miners will place their transactions where the reward per byte (size of the block) is at a maximum, so they can make the most of the limited space inside a block.

#### Example

If a transaction takes up 8B, and has a reward of 20, while another transaction has a size of 1B, but a reward of 5, the 1B transaction will have higher priority as it takes up the least amount of space but gives a lot of value in return.

---