# Digital Signature

A digital signature is a combination of the **private key** and the **transaction data** itself. This is useful in cryptocurrency because it allows someone to show that they are the correct recipient without revealing their private key. This is also unique to every transaction as transaction data is always going to be different - this means that people can't use the same digital signature for other transactions to pretend to be somebody else.

---

## How do they work

To create a digital signature, the private key, transaction data as well as a random number is used.

To confirm whether a legit private key was used to generate the digital signature, the digital signature, transaction data, and the public key are used together, and the result will then show whether the private key used is legit.