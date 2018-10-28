## Qu'est-ce que les smart contracts?
---

### Principe 

La blockchain Ethereum dispose d'une capacité singulière vis-à-vis des autres blockchains,
Elle peut être programmée à l'aide d'un langage spécifique: Solidity. C’est un langage de programmation «complet» (turing-complete), c'est-à-dire qu'il permet d’exécuter l’ensemble des fonctions utilisés pour développer une application moderne. 

Cela permet de programmer des engagements sur la blockchain Ethereum. Ceux-ci peuvent simple, comme engager une transaction ou plus complexe, car constitué de plusieurs actions en série ou parallèle. 

Lorsque les conditions d’exécution de ces engagements sont réunies, ces contrats s’exécutent automatiquement sur la blockchain, en prenant en compte l’ensemble des conditions et des limitations programmés à l’origine.

Un contrat de prestation de service entre deux entités peut aisément se modéliser sous la forme d'un smart-contract.

La première souhaite rémunérer la seconde en paiement de la prestation, ce contrat est formalisé dans la blochain Ehthereum par la création d'un engagement de type smart-contract. La somme correspondante est alors mise en gage sur la blockchain. Lorsque la prestation est réalisée, l'engagement vérifie automatiquement que les conditions fixées ont bien été remplies et le cas échéant, verse la somme gagée. En cas de manquement aux stipulations du contrat, la partie gageante se voit restituer la somme.

Les transactions effectuées sont publiques, il s'agit du principe de publicité. La bonne exécution du contrat peut ainsi être vérifié, n’importe quelle partie qui dispose du code source du contrat peut vérifier que le contrat a bien été enregistré.

La blockchain prodigue une sécurité élevée, l'une de ses limites est la vulnérabilité à l'attaque des 51%. Voir [sécurité de la blockchain](./blockchain_securite.md/).

Les données qui sont enregistrées dans la blockchain y sont enregistrées de manière immuable: l’historique est conservé depuis l’origine. Un engagement est irrémédiablement enregistré dans la blockchain.

Mettre hors ligne une blockchain nécessiterait d'arrêter simultanément tous les nœuds de celle-ci, ce qui est virtuellement. C'est donc un système que l'on peut considérer comme fiable.

{% hint %}

En résumé les smart-contrats permettent d'engager des accords entre deux parties sans que l'une ne puissent entraver son exécution, mais également des applications décentralisées.

{% endhint %}

### Limites

Se pose alors la question de la validation des conditions d'exécutions. En effet, puisqu'elle interagit avec le monde physique, le smart-contract doit parfois disposer de capacitées matérielles. Pour cela deux possibilités:

[//]: # (TODO: Check if correct)

* Condition d'exécution interne:
    Lorsque les conditions d'executions ne nécessitent pas une interaction physique avec l'environnement, les conditions sont inscrites dans la blockchain. Le contrat est exécuté dès que les conditions sont remplies et que la date d'exécution est atteinte.

* Condition d'exécution externe: 
   Lorsque les conditions d'exécution sont extérieures à la blockchain comme la réalisation d’une prestation, survenance d’un événement… etc. Dès lors, le recours à un tiers de confiance, appelé  «oracle» est nécessaire. Il lui est délégué l'observation des ces évenements étrangers et l'écriture des conditions dans la blockchain.

{% hint style='danger' %}

La principale limitation inhérente à la technologie blockchain est la lenteur du réseau, contrepartie de sa sécurité. 

{% endhint %}

### Dans le cadre du vote: 
Exemple avec l'utilisation d’un service d’oracle: 

Le recours à un service d'oracle nécessite un nombre important de participants. Chaque protagoniste vote pour le résultat qu'il juge exact et le résultat est confié au consensus. On peut citer en la matière le projet Oraclize. Dans le cadre du vote cela sous-entend de confier un nombre de propositions au consensus qui détermine les éléments valides.

Une proposition est dans ce cas de figure un smart-contract classique dont les conditions fixent le cadre d'application. Une fois ces conditions validées, le contrat voit son exécution programmée.

Ce système présente une limite et nécessite une vigilance particulière. En effet l'interruption du contrat (et donc de l'exécution de la proposition) est en pratique impossible, sauf si cette condition d'interruption a été prévue dès l'origine.
