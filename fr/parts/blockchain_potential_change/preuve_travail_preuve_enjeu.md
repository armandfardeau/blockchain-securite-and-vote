## Preuve de travail vs preuve de l'enjeu
---

Une blockchain est donc un registre distribué chiffré,et répliqué dans tous les noeuds du réseau, qui contient les chaînesd’ordre permettant, grâce à l’obtention d’un consensus,de gérer la confiance sans institution externe .

### Concernant la preuve de travail :

De l'anglais proof-of-work.

Nous avons vu précedemment que la chaîne est constituée d'un ensemble de blocs de données contenant des informations ainsi qu'un horodatage. A chaque transaction, ces blocs sont intégrés à la chaîne.
 
Afin de garantir son intégrité, cette chaîne est chiffré et doit êtrecertifiée. 

Pour certifier la transaction, de puissants ordinateurs constitués de noeuds en réseau réalisent des calculs cryptographiques.

Le travail global de certification se nomme « preuvede travail » (proof of work). 

On appelle les machines (ou institutions) quieffectuent ce travail de certification des « mineurs » de l'anglais mining.

L'objet cryptographique crée par le mineur est la preuve du temps passé à la certification, il constitue la preuve de travail. 

Il est essentiel de garantir la nature réelle du travail des parties prenantes afin de préserver le consensus.

Fruit d'une invention d'Adam Back, inventeur du protocole Hashcash, elle évite unclonage facile qui aurait pour conséquences de pouvoir controller la blockchain de manière rétroactive.

Le mécanisme est même plus sophistiqué :à intervalles de temps réguliers, la difficulté augmente.

![La difficulté de hash blochain](../../images/difficulty.jpeg)

> Mesure relative de la difficulté de trouver un nouveau bloc. La difficulté est ajustée périodiquement en fonction de la puissance de hachage déployée par le réseau de mineurs.
>
> Source: blockchain.com 



La mise en concurrence est la méthode utilisée pour motiver à la certification, ainsi le premier mineur à valider un nouveau bloc sera récompensé.

Concernant le bitcoin, la tâche de certification était à l'origine accessible par les particuliers grâce à l'utilisation des cartes graphiques, dont la puissance pour le type de calcul nécessaire à la cetification est supérieure.

Depuis des mineurs spécifiques sont apparus pour réaliser la preuve de travail et les cartes graphiques grand-public sont délaissés car non compétitive.

Car plus la taille des chaînes augmente, plus la puissance de calcul doit augmenter. Cette relation d'interpendance a chassé les particuliers de la course à la certification et se sont désormais des institutions qui ont pris le relais.

![La ferme de calcul bitfarms](../../images/bitcoin_farm.jpeg)

> La ferme de calcul bitfarms
>
> Source : bitfarms.io



En Août 2018, il y avait 9 503 noeuds de traitement de la blockchain bitcoin dans le monde.



![global bitcoin nodes distribution](../../images/GLOBAL_BITCOIN_NODES_DISTRIBUTION.png)

> Global bitcoin nodes distribution
>
> Source : bitnodes.earn.com


Les services de mining sont disponibles dans le cloud à travers le cloud-mining, ce qui reste néanmoins un modèle plus orienté vers les entreprises ou les grandes organisations que les particuliers.

### Concernant la preuve de l’Enjeu :

De l'anglais proof-of-stake.
