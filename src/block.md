# Block

Each *block* in a [blockchain](/blockchain.html) records a large number of transactions that have taken place (for example, in Bitcoin it's around 2400)

At the end of each block, there needs to be a 'proof of work' where each result in a block is chained together, and 'miners' find a value that returns a hash that has a set number of 0s at the beginning (which can be changed depending on number of miners)

Each block must contain the hash of the previous block in the header - making a chain. Thus, if you want to change an earlier block, you need to calculate the proof of work for all subsequent blocks too. And at that point, you are simply racing against other miners - if you have less than 50% of the share of resources in terms of mining, then you won't be able to keep up (in terms of trying to fake data)

The first block in the chain (without any previous hash) is called the genesis block.

Whenever the miner gets the proof-of-work, they then get paid a share of the cryptocurrency (thus giving them an incentive to mine)