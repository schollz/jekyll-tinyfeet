---
layout: post
title: How does Bitcoin work? (Yes, yet another description of how Bitcoin works)
tags: [bitcoin, currency, explainations]
date: 2015-08-16
comments: true
landing: true
---

## Why isn't USD good enough anymore?

Standard currencies like USD, Yen, Euro's all have a central bank associated with them that can print and distribute money at their whim. Bitcoins are a special type of currency - a cryptocurrency that is completely decentralized. Instead of a bank manager looking over the system and injecting cash when needed, the decentralized currency system monitors and regulates itself! How is this possible?

![Banks do a lot](/content/images/2015/07/peter-c-vey-bank-grill-new-yorker-cartoon.jpg)

## How to make a decentralized currency?

The decentralized Bitcoin currency operates with a security system that is inherent to its creation. Security is mainly provided through [RSA encryption](http://en.wikipedia.org/wiki/RSA_(cryptosystem)) (widely used on the internet) and hashing. [Hashing](http://en.wikipedia.org/wiki/Hash_function) is basically a irreversible and unique encryption of any string of number and letters. For instance, "The quick brown fox." becomes "b61e52d47fe1c856c5f0fec57b560b794adf6561" after a SHA-1 hash while a sentence with only one difference ("The quick, brown fox.") becomes "cd857b0849271ecfc0ba58e5db27dcba8e8d054f". Hashes are useful because their randomness gives no inclination to the content of the original text, and the process of reversing a hashed value into its original string is essentially impossible.

## The three problems, and their solutions is the essence of Bitcoin

However, a system of a decentralized cryptocurrency necessitates security beyond universal encryption. The **first major problem is how to prevent malicious attacks onto a ledger which is available to everyone and anyone on the peer-to-peer network?** The solution to this is hashing the first transaction and then propagating the previous hash with all following transactions. Thus the true ledger can easily be checked by hashing every transaction. If the ledger had been altered in any way, the resulting hash would not match the previously accepted versions of the ledger and it would be rejected.

The **second problem is how to infuse money into a decentralized cryptocurrency system - where does the money come from?** In the Bitcoin system, a single Bitcoin is injected to the system each time that a hash of a transaction is solved. To be "solved", Bitcoin requires the hash to have certain parameters, i.e. the hash must start with the letter "B". Different hashes are obtained by adding in a "fudge number" in addition to the current transaction and the previous hash. Changing the fudge number will randomly change the resulting hash, but does not change any of the important transaction details. Thus, every peer on the network changes the fudge number until their hash fits those parameters and is considered solved. This hashing, often called "mining", provides security of the ledger but takes significant computational (and energetic) costs. These costs are alleviated by awarding the hash-solver in the network the Bitcoin.

![Security is a main concern for the Bitcoin system](/content/images/2015/07/eric-lewis-guess-your-atm-password-booth-at-carnival-new-yorker-cartoon.jpg)

Finally, **a third problem that needs to be overcome is how to prevent double-spending?** In the currently described system, a user may spend Bitcoin (by having the hash of their transaction solved) and then spend the same Bitcoin before the previous one propagates through the network - essentially creating two ledgers with the same Bitcoin. However, this is solved in Bitcoin quite simply because hashing is a hugely difficult process - it would take a single computer almost 98 years to solve one hash - so it is very unlikely in the first place that a single person could manifest an attack on their own. If the situation arises however, the branched ledgers will be resolved on the next hash, such that the longest branch is accepted as the "true" ledger and all other ledgers and their transactions are invalidated. Thus it is commonly purported that one should wait 10-20 minutes before trading goods with Bitcoins to ensure the transaction is propagated and validated in the system.

**Bitcoin is really the solution to these main problems. As a technical theory it is quite elegant, but it has so far managed to produce a viable, practical currency as well!**

