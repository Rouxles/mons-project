# SSH and PuTTYGen

PuTTYGen is used to generate private and public keys using the SSH-2 algorithm.

These private and public keys are used for the output locks - locks used to identify the address that the transaction is aimed for. 

When each transaction is created, it takes one output (that someone owns) and creates more outputs out of that (potentially addressed to other people). When an output is created, a lock is placed with it addressed to a certain person, and they can only access the outputs of that if they can unlock the lock - essentially only if they have the private key to ensure that the person trying to unlock the outputs is the person they say they are.

