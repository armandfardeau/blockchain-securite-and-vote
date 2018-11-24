## What are smart contracts?
---

### Principle

The Ethereum blockchain has a unique capacity compared to other blockchains,
It can be programmed using a specific language: Solidity. It is a "complete" programming language (turing-complete), i.e. it allows to execute all the functions used to develop a modern application. 

This allows you to schedule commitments on the Ethereum blockchain. These can be simple, such as initiating a transaction, or more complex, because they consist of several actions in series or parallel. 

When the conditions for the execution of these commitments are met, these contracts are automatically executed on the blockchain, taking into account all the conditions and limitations originally scheduled.

A service contract between two entities can easily be modelled as a smart-contract.

The first wishes to remunerate the second in payment of the service, this contract is formalised in the Ehthereum blog by the creation of a smart-contract type commitment. The corresponding amount is then pledged on the blockchain. When the service is provided, the commitment automatically verifies that the conditions set have been met and, if necessary, pays the sum pledged. In the event of failure to comply with the provisions of the contract, the pledging party shall be reimbursed the sum.

The transactions carried out are public, this is the principle of disclosure. The proper execution of the contract can thus be verified, any party who has the source code of the contract can verify that the contract has been registered.

The blockchain provides high security, one of its limits is the vulnerability to attack of 51%. Voir [sécurité de la blockchain](./blockchain_securite.md/).

The data that is recorded in the blockchain is recorded in an immutable way: the history is kept since the beginning. A commitment is irrevocably recorded in the blockchain.

Offlining a blockchain would require stopping all nodes of the block simultaneously, which is virtually impossible. It is therefore a system that can be considered reliable.

{% hint %}

In short, smart-contracts make it possible to enter into agreements between two parties without one of them being able to hinder its execution, but also decentralized applications.

{% endhint %}

### Limits

This raises the question of the validation of the execution conditions. Indeed, since it interacts with the physical world, smart-contract sometimes has to have material capacities. There are two possibilities for this:

* Internal execution condition:
    When the execution conditions do not require physical interaction with the environment, the conditions are recorded in the blockchain. The contract is executed as soon as the conditions are met and the execution date is reached.

* External execution condition: 
   When the conditions of execution are external to the blockchain such as the performance of a service, the occurrence of an event... etc., the use of a trusted third party, called "oracle" is necessary. It is delegated to him the observation of these foreign events and the writing of the conditions in the blockchain.

{% hint style='danger' %}

The main limitation inherent in blockchain technology is the slowness of the network, in return for its security. 

{% endhint %}

### As part of the vote: 
Example with the use of an oracle service: 

The use of an oracle service requires a significant number of participants. Each protagonist votes for the result he or she considers to be accurate and the result is entrusted to consensus. One example is the Oraclize project. In the context of the vote, this implies entrusting a number of proposals to the consensus that determines the valid elements.

A proposal is in this case a classic smart-contract whose conditions set the framework for its application. Once these conditions have been validated, the contract is scheduled for execution.

This system has a limit and requires particular vigilance. Indeed, the interruption of the contract (and therefore of the execution of the proposal) is in practice impossible, unless this interruption condition was foreseen from the outset.
