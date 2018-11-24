## What is the blockchain?
---

The term blockchain refers to both the system and the technology behind it.

The blockchain is known mainly to the general public as the technology used by Bitcoin.

Invented in 2008, the Bitcoin is originally a prototype designed to demonstrate the possibility of creating a cryptocurrency whose mechanism is based on a distributed register distributed among multiple nodes of a network.

Due to their intrinsically open-source nature, encryption algorithms are an additional argument for confidence in this system.

**If the Bitcoin has benefited from such media exposure, it is because it is a limited volume currency that is outside the current benchmark. But above all, it is a currency that challenges the role of banking institutions and states as trusted third parties and legitimate entities to issue and regulate money.**
 
### The three pillars of the blockchain

The blockchain is based on three pillars: two are technological, namely asymmetric cryptography and distributed systems, and the third is sociological.

#### 1. Cryptography

It is based on the concept of a key. 
There are two types of keys: symmetrical and asymmetrical. 

The former have been known since antiquity and the latter were first introduced in the 1970s.

The second is essential to blockchain technology because it ensures 
the authenticity of the sender of the message. The sender uses his private key to code a message that the recipient can decode with the sender's public key. The symmetric encryption method has the advantage of being inexpensive in terms of computing power, and of remaining very secure. Unfortunately, it has its limitations:

> The disadvantage is that to encrypt an n-bit message, you must first have exchanged an n-bit key with the recipient of the message, and this by an absolutely secure means, otherwise encrypting becomes unnecessary. 

> Claude Shannon, Communication theory of secrecy system

Instead of this method, asymmetric encryption is preferred, which makes it possible to bypass the obstacle of the common key for all stakeholders.
Indeed, in the context of asymmetric encryption, two keys are present: 
private and public. The key that is chosen private is never transmitted to anyone while the key that is chosen public is transferable without restriction.

This technique allows:

* ##### Encryption
 
    One of the roles of the public key is to enable encryption. It is therefore this key that a first subject will use to send encrypted messages to a second subject. The other key - the secret information - is used to decipher. Thus, the second subject, and only the second subject, can read the messages of the first subject. 

    **The knowledge of one key does not allow the other key to be deduced.**

* ##### Origin Authentication

    The use by one of the subjects of his private key on the condensate of a message will allow the latter to verify that the message comes from the expected interlocutor and to prevent usurpation: 
        he will apply the public key that his interlocutor provided him on the condensate (encrypted condensate with the private key of the other subject) and thus find the original condensate of the message.
        
        It will therefore be sufficient for him to compare the condensate thus obtained and the actual condensate of the message to know if his interlocutor is really who he claims. It is on this mechanism in particular that the digital signature works.

#### 2. Distribution

The Internet happens to be one of the most beautiful proofs of a distributed system, no need for a single telecommunications operator so that anyone, anywhere in the world, can connect to the Internet.

#### 3. Distributed consensus

To understand the concept of distributed consensus, the example of an operation to combat drug traffickers seems to us to be the most appropriate. 

Imagine a city fighting crime, especially a powerful cartel. As part of an operation to combat drug trafficking, all the police forces in the region are working together to destroy criminals.

The different police organizations must all attack together to take advantage of the surprise effect. Otherwise they would be overwhelmed and traffickers would risk taking advantage of the confusion to escape. 

They therefore had to coordinate the date and time of the attack, and, as they could not all meet, they delegated the role of messenger to some in order to limit the comings and goings.

Unfortunately, in such a corrupt city, no one can be trusted and some police officers are actually undercover criminals whose objective is to thwart the attack.

For example, one of them may tell half of the police forces that they must attack at a given date and time, and the other half that they must withdraw, a disorganization that will not allow them to benefit from the surprise effect and numerical superiority.

**The great novelty brought by the blockchain is to propose a system that allows to get rid of this hierarchical authority.**

In essence, each police force can only send one order at a time, associated with a timestamp.

Most importantly, however, the orders are aggregated to each other and then encrypted, forming a chain stored in a "transaction ledger", which is redistributed to all the police services involved. 

A chain is thus formed, containing a hash of all previous orders.

Thus, if a messenger receives the information "The search will take place tomorrow at 4:00 p. m.", and decides to pass it on to only half of the others and send a different schedule to the other half, he will change the value of this hash.

As other messengers share information with all police forces involved, it will be possible to determine inconsistent chains and identify corrupt ones simply by comparing the value of hashes.

This of course implies that the number of honest messengers is greater than the number of corrupt ones.

### Consensus methods:

| Consensus type | Description | Advantages | Disadvantages | Blockchain type|
|:-----------------:|-------------|-----------|---------------|-------------------|
| Proof of work (PoW) | Miners' computers are made available to solve a complicated mathematical problem. The first one to find a solution wins the reward for the next block in the chain. | Secure, proven and robust. | High electricity and computer equipment consumption. | Public
| Proof of stake (PoS) | Transaction validators must pledge possession of cryptomone to receive a reward. If a node is malicious, it may lose its pledge to honest validators. | Low consumption of energy resources. | Little tested on a large scale. | Public |
| Practical Bizantine Fault Tolerance (PBFT) | Consensus whose list of validators is known at the outset and can tolerate up to 1/3 of compromised nodes (disconnected or malicious). | Fast and efficient group consensus building. No fork or chain reorganization. | | Private |
| Proof of authority |  Consensus whose list of validators is known at the beginning and which validates a block in turn. This type of consensus can tolerate up to 49% of malicious or disconnected nodes. | Quick group consensus. | | Private |
