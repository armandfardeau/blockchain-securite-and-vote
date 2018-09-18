## Vers une normalisation ?
---

> 10% du PIB mondial en 2025 proviendra d’activités utilisant la blockchain.
> 
> Ravi Jhawar, le responsable du projet au sein du GIE de l’Anec

### Une régulation par la normalisation
Le Luxembourg, par le biais de l’Ilnas, participe à la création d’une norme technique internationale pour encadrer la blockchain. 

Dans un [livre blanc](../../sources/wp_blockchain_ilnase.pdf), l'organisation espère initier une démarche et s'imposer comme un acteur de la régulation à travers une norme ISO.

L'objectif est d'encadrer la gouvernance des blockchains afin de peser dans les enjeux économiques et écologiques qui la concerne. 

Cette normalisation se confronte nénamoins à la volonté d'indépendance et de décentralisation, base fondatrice des technologies blockchains. 

Néanmoins la mise en place d'une norme peut impliquer une meilleure régulation énergétique en imposant par exemple l'origine renouvelable de l'électricité nécessaire au fonctionnement de la technologie.

### La standardisation pour lutter contre la consommation et l'obsolescence des moyens de productions.

Le terrain de réduction de la consommation énergétique de la blockchain se déssinent lorsque l'on évoque la standardisation ou la normalisation.

Il s'agit de la standardisation des algorithmes et celui du matériel polyvalent.

Ces deux directions d'optimisation ne sont en fait qu'une seule et même voie : un standard algorithmiques signifie un matériel dédié adapté, et donc une optimisation plus importante car les investissements de Recherche & Développement seraient focalisés sur un seul type de de matériel.

Les blockchains fonctionnant sur la méthode de preuve de travail ont en commun l'utilisation d'un algorithme de hashage. Celui de Bitcoin est nommé Hashcash.

En recherchant un alogorithme plus économe pour remplir cette fonction, la blockchain pourrait voir son coût écologique se réduire et se présenter comme une alternative viable à grande échelle.

Afin de miner, les individus ou institutions mettent à disposition du matériel afin de réaliser des calculs. 

Sur certaines blockchains, comme bitcoin, il est inutile et non-rentable de s'essayer à la chose avec du matériel classique et 

Ce mode de calcul est réservé à des blockchains plus récente ou bénéficiant de moins d'engouement.

Les mineurs professionnels ont recours à du matériel performant, qui exclut les mineurs amateurs de la course à la rémunération. (Dans le cadre de la preuve de travail seulement.) Ceux ci étant bien trop lent pour valider les transactions face à ces sprinteurs.

Le minage est divisé entre deux technologies, les puces dédiées : **FPGA / ASICS** et les puces généralistes **CPU / GPU**.

Les mineurs ASICS ET FPGA sont majoritairement utlisées dans le calcul SHA256 (Bitcoin), tandis que les CPU / GPU sont plutôt utilisés sur des cryptomonnaies plus récentes.

La difficulté doit augmenter au fil des avancées technologiques afin de maintenir la complexité de calcul au sein d'une blockchain, c'est ainsi que certains algorithmes étaient résistants aux ASICS grâce à une importante utilisation de la mémoire, composant couteux, rendant ce matériel peu compétitif.

Mais 2017 a marqué un tournant dans l'utilisation de ces cartes avec une amélioration substancielle de ces modules mémoires. La solution pour maintenir la complexité fut de modifier les algorithmes, rendant le matériel obsolète car les fonctions d'un mineur ASICS sont gravées à même le silicium. On parle alors de fonctions cablées.

Ces fonctions cablées se retrouvent dans d'autres architectures de puces, comme les GPUs.

**Un coût économique et écologique important pour garantir la sécurité et la scalabilité de ces blockchains.**

Pour comprendre pourquoi les puces sont rendues obsolètes il faut intégrer  que la différence entre un CPU et un ASIC (ou entre un CPU et un GPU) réside dans le fait quer le CPU est une puce programmable, et doté d'une grande polyvalence dans son utilisation au prix néanmoins d'une performance moindre.
 
 UN GPU ou un ASIC est une puce spécialisée, dont les performances sont excellentes dans l'accomplissement des taches pour lesquels elle est programmée, mais qui sont, plus réduites en nombre que pour un CPU. 
 
 Par example, pour un GPU, spécialisée dans la représentation graphique, l'affichage d’un maillage 3D texturé à 60-100 frames par seconde.
 
 Cette performance permet d'obtenir des meilleures performances en terme de calcul brute sur ces taches précises, mais également une consommation électrique plus faible.
 
 Cette amélioration de performance est rendure possible par le fait d'insicrire en dur, de cabler les fonctions nécessaire à la translation, rotation etc...
 
 Pour un mineur ASIC, cette spécialisation se traduuira dans une performance inégalable dans la résolution d'un algorithme de chiffrage par exemple. Mais il n’est pas possible d’utiliser un ASIC spécialisé dans le calcul de hashs SHA256 pour du KECCAK et inversement.
 
 
Dans ces tendances, une solution intermédiaire a vu le jour et exploite le meilleur des deux mondes : le FPGA.

#### Le FPGA.
Les FPGA (Field-Programmable Gate Array) sont des circuits intégrés en silicium reprogrammables. 

Reprogrammer un FPGA consiste à redéfinir le circuit intégré lui-même pour implémenter la fonctionnalité souhaitée, au lieu d'exécuter une application logicielle. 

On peut voir le FPGA comme une puce qui simule au plus bas niveau une puce spécialisée.  

Les FPGA sont particulièrement utilisé pour simuler un mineur ASIC dans la phase de préproduction afin de tester le modèle et ajuster les schémas logique. Lorsque le fonctionnement est jugé suffisant, le schéma est alors figé pour produire un mineur ASIC. 

Les mineurs FPGA offrent des performances légèrement moindre que les mineurs ASICS. On note aussi que la logique de programmation d’un fpga nécessite des compétences poussées et peu répandues.

Malgré ces désavantages, des cartes FPGA aux capacités de calcul titanesque sont en train de se développer pour répondre aux besoins du machine-learning et du deep-learning. 

Ces cartes permettent d'envisager une continuité d'utilisation future malgré les forks et les évolutions de l'algorithme, ce qui permet de limiter les coûts et de limiter l'impact écologique dû à l'obsolescence du matériel.
