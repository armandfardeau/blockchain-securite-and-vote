## Participatory democracy
---

These are a combination of the concepts of participatory democracy and representative democracy.
 
 * "Delegated democracy" (liquid democracy) is a form of democracy where voting power is entrusted to a delegate rather than a representative. This system can be considered as a synthesis between direct democracy and representative democracy.
 
 * "Participatory democracy" which evokes the idea of citizen involvement and participation in public debate but also in political decision-making. This term, which is very much in vogue, often refers to extremely varied realities.

## First experiments

* ### L'Open Vote Network

**In A Smart Contract for Boardroom Voting with Maximum Voter Privacy, Patrick McCorry, Siamak F. Shahandashti and Feng Hao present the first implementation of a decentralized and self-accounting Internet voting system with maximum voter confidentiality using the blockchain. 

**The voting in this example is "open ballot" and is suitable for board elections. It is written as a "smart-contract" for Ethereum. 

Unlike previous experiments on electronic voting protocols, the researchers were able to implement a system that does not rely on any trusted authority to calculate the count or to protect the voter's privacy. 

The **Open Vote Network** is an autonomous voting network and each voter is responsible for the confidentiality of his or her vote.
 
With such an implementation, this vote could only be compromised by total collusion involving all other voters.

The voting protocol is guaranteed by the consensus mechanism that also secures the Ethereum blockchain. 

The implementation of this network was carried out on Ethereum's social test network to 
demonstrate its feasibility and has shown that its implementation can be possible with a minimum of configuration for elections and at a cost of $0.73 per voter. 

The cost can be considered reasonable as long as this vote ensures maximum protection of the elector's privacy and is publicly verifiable. 

This is the first implementation of a decentralized Internet voting protocol based on an Internet voting system.

It uses the Ethereum block chain not only as a public bulletin board, but more importantly, as a consensus calculation platform that enforces the rules for the correct execution of the voting protocol.

Although the number of subjects tested may seem trivial, this is a first initiative that needs to be pursued on a larger scale. In future work, the researchers have stated that they will study the feasibility of exploitation on a national scale.

The point raised by this study is that if such a perspective is made possible, it will almost certainly require a dedicated block chain. 

For example, it may be a chain of Ethereum-type blocks that only stores the electronic voting contract. 

The new block chain can have a larger block size to store more transactions on the chain and can be maintained in a centralized manner similar to RSCoin.

* ### The first blockchain-based election took place in Sierra Leone

> "Sierra Leone wishes to build trust with voters in a controversial election, in particular by examining how the election will be perceived publicly after the elections. By using the blocking chain as a means of immutably recording ballots and results, the country hopes to create legitimacy around the election and reduce the impact of opposition parties," he said.  
>
> Leonardo Gammar in "Sierra Leone just held the first blockchain-based elections."

On March 7, 2018, a blockchain-based vote was held in Sierra Leone with a 70% participation in one blockchain.

Agora technology, created by Leonardo Gammar, anonymously stores votes in an unchanging register, providing instant access to election results.

> Anonymous votes/bulletins are recorded on Agora's blocking chain, which will be accessible to the public for any interested party to review, count and validate. This is the first time a government election has used blockchain technology.
>
> Leonardo Gammar, Agora

This experience stems from a major movement towards transparency and anti-corruption in Sierra Leone, particularly in the context of elections, the results of which are often controversial.

This experiment will test the impact on the perception of integrity in the context of the election. In this way, citizens and stakeholders hope to create legitimacy around the election and reduce the impact of opposition parties. 

Although this is only a proof of concept (POC), it is not a complete electoral register, but rather a plurality of votes in acceptable quantities.

It is fascinating to see the technology being implemented in Sierra Leone, a country of about 7.4 million people. 

The ultimate objective is to reduce the costs of voting by eliminating paper ballots and reducing corruption in the voting process.

This first experiment demonstrates the feasibility of the operation in a country of several million inhabitants where corruption and crime are high.
 
 Its creator takes as an example the backtracking of many countries on electronic voting to advance the inevitability of blockchains in voting decision-making processes, arguing that there are no other verifiable and fully transparent end-to-end voting systems for this future.

However, it is a question of putting this experience into perspective, because an election in a country is not yet a massive movement. However, Gammar and his team have announced their intention to expand their product to other African countries and the rest of the world.

* ### DEMOCRACY EARTH project

![Logo de la Democracy Earth Foundation](../../images/democracy-earth.png)
> Democracy Earth Foundation logo

Democracy Earth Foundation (DEF) is a US non-profit foundation that builds a "liquid democracy" oriented governance platform based on an open source blockchain. 

The DEF published version 1.0 Alpha of the governance platform, Sovereign, in May 2017 and its white paper, The Social Smart Contract, in September 2017. During the referendum for peace in Colombia, the foundation conducted a symbolic vote among the diaspora of approximately 6 million Colombian expatriates. The pilot project allowed people to vote separately on different parts of the referendum and to delegate their vote to representatives, with the results of the symbolic vote revealing important nuances in voters' preferences that were not taken into account during the referendum. The pilot project actively shows how participatory democracy reduces polarization, powerlessness and voter apathy.

#### The implementation of the vote in the DEF project

The voting token aims to be a standard for digital democracy capable of interacting with other tokens, by establishing a common language for the governance of organizations based on the block chain. In the context of liquid democracies, a range of voting operations is permitted:

* Direct voting: a user has the right to use his or her tokens to vote directly on issues such as in a direct democracy.

* Basic delegation: a user can delegate votes to a representative. As long as the latter has access to these tokens, he can use them to vote on behalf of the former.

* Limited delegation on topics: A user may delegate votes to another on the specified condition that he/she may only use these tokens on issues bearing a specific label. If the delegation specifies that delegated votes can only be used for decisions on the subject of "environment", then the representative may not use them elsewhere. This potential for representation can be used to delegate a vote to an expert on a particular subject.

* Transitional delegation: If a user has received votes from another user, they can then delegate them to a third. This generates a chain of delegations that helps to empower specific actors within a community. This character can be disabled by the first user if he/she wishes.

* Overriding vote: A user may delete the result of his representative's vote if he has changed his mind, so that he can exercise ex post control of his delegated opinion.

* Public voting: Often referred to as the golden rule of liquid democracies, anyone who delegates has the right to know how his or her delegate voted on a given issue with his or her vote. In the same way that the votes of Congress members are public, on liquid democracies, delegates competing on a given subject are encouraged to build a public reputation based on their voting results in order to attract more delegations.

* Secret vote: A method capable of guaranteeing voting transactions that are not traceable to the voter. This is essential in the context of public elections held among large populations at high risk of coercion. Even if the perfect secrecy over the voting transaction is achieved, users can still be identified through fingerprints with the exposed metadata. For this reason, research on integration with blockchains designed for proven anonymous transactions is encouraged. The DEF is continuing its research on the integration of secret votes with the following blockchains:
    * Ethereum: uses pre-compiled contracts for addition and scalar multiplication on the elliptic curve alt_bn128, for matching controls, which allow zk-SNARKs.
    * ZCash: implements secure transactions using zero disclosure evidence of knowledge
    * Monero: use circle signatures with stealth addresses.
 
The transaction costs necessary for the validation of the vote may either be subsidised by the implementing body or paid directly by the voters.
   
{% hint %}

DEF uses a zero knowledge proof system to guarantee the identity of the voter without publicly registering them in the blockchain. This is a major step forward in the voting process using this technology. Thus, the problem of confidentiality in the context of the secret ballot finds a first element of answer.

{% endhint %}
