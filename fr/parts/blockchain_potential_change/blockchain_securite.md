## Quid de la sécurité de la blockchain ?
---

### Les garanties de la blockchain en matière de sécurité:

Il n'existe pas de technologie sûre dans la mesure où la sécurité et la sureté sont un idéal, pas un absolu. Mais il est possible de s'approcher de cet idéal, on peut d'ailleurs considérer que la blockchain répond à ces impératifs dans la mesure où elle assure les points suivants:

 * La disponibilité: Les données étant distribuées et décentralisées, elles sont disponibles tant qu'un nœud est en mesure de transmettre le registre. 
 
 * L'intégrité: le mécanisme de consensus est conçu pour permettre aux informations d'être intégrées et conservées sans que celles-ci ne soient altérées. Le pré-requis à cette disposition est qu'un nombre suffisant de nœud soit connecté au réseau et que les conditions permettant une attaque des 51% ne soient pas atteintes.
 
 * La confidentialité: La confidentialité est un point complexe concernant la blockchain puisque les données sont disponibles publiquement pour garantir la transparence.
 
  Néanmoins cette confidentialité peut être rendue possible par l'implémentation d'un système de preuve à divulgation nulle de connaissance. Les protocoles sans connaissance permettent le transfert de ressources à travers un réseau distribué, peer-to-peer blockchain, en toute confidentialité. Dans les transactions régulières en chaîne de blocs, lorsqu'un actif est envoyé d'une partie à l'autre, les détails de cette transaction sont visibles pour toutes les autres parties du réseau. En revanche, dans une transaction sans connaissance, les autres parties ne savent pas qu'une transaction valable a eu lieu, mais aucune information sur l'émetteur, le destinataire, la catégorie d'immobilisations et la quantité n'est divulguée. [Voir Gestion de l'identification et confidentialité](./identity_and_confidentiality.md)
 
 * La traçabilité: Parce qu'elle est basée sur un empilement de blocs cryptographique, la blockchain permet d'enregistrer l'intégralité des transactions et de remonter au bloc zéro, assurant la meilleure des traçabilités.
 
 * L'authentification: Pour s'assurer de la bonne identité d'une transaction, l'émetteur signe celle-ci à l'aide de sa clé privée qui «tant qu'elle n'est pas connue assure la véracité de la transaction». 
 
 * La non-répudiation et l'imputation: Par le biais de la validation basée sur le consensus, la blockchain permet nativement la non-répudiation des données. Quant à l'imputation, chaque mineur certifiant une transaction est authentifié sur le réseau, il est donc possible d'identifier un mineur fautif et de le disqualifier.


---
### Les menaces qui pèsent sur la blockchain en matière de sécurité:

Selon Patricia Egger et Dusko Karaklajic dans La sécurité du blockchain, des menaces pèsent sur l'écosystème naissant en raison de l'immaturité et la complexité de la technologie.

En effet, les nombreux algorithmes de consensus disponibles, les types de blockchain et protocoles cryptographiques complexes sous-jacents rendent la technologie difficile à appréhender.

L'absence de normes et de réglementations sur la technologie du blockchain constitue également un risque. Ces vides juridiques sont un terreau fertile au piratage et à la manipulation frauduleuse rendent la technologie encore peu crédible pour des usages sérieux. 

Le risque le plus important demeure la croyance dans la sécurisation absolue autour de la blockchain bien qu'elle repose sur des mécanismes cryptographie fiables et éprouvés. Cette sécurisation ne sera jamais complète par nature: les protocoles cryptographiques ont leurs limites et la sécurité globale intègre également les éléments périphériques, le risque humain est ainsi toujours présent. En ce dernier point, la blockchain apporte une nouvelle manière de traiter certaines données mais n'affranchit pas des démarches classiques en matière de sécurité des systèmes d'informations.

En outre la blockchain est sensible à des attaques particulières, comme l'attaque de type Golfinger.

#### Attaque des 51% ou attaque Goldfinger

Une attaque des 51% cible les blockchains basée sur la preuve de travail et preuve de l'enjeu.  

Le but de cette attaque est d'empêcher les validations des transactions et de paralyser le réseau, ou de manipuler l'historique pour valider deux fois une transaction sans pour autant que la dépense ne soit effective. 

La validation des blockchains se fait grâce aux minages.

Afin de se garantir une rémunération dans le cadre d'une blockchain fonctionnant sous la méthode de la preuve de travail, les mineurs se constituent en groupe (ou pools), de façon à disposer d'une puissance supérieure et de mutualiser les coûts. Ils partagent alors les efforts ainsi que les gains.

Mais le danger d'un groupe disposant d'une puissance trop importante est qu'il peut réaliser une attaque des 51%.

En effet l'un des principes fondateurs de la blockchain est que le calcul est distribué entre tous les nœuds où le calcul est validé par la méthode de consensus. Ainsi si un seul individu introduit une erreur de calcul volontairement ou falasieusement, les autres mineurs vont automatiquement disqualifier son travail et son bloc va demeurer orphelin et ne sera jamais intégré. Ainsi seul, il ne peut pas nuire.

{% hint style='danger' %}

Lorsqu'un groupe de mineur dispose d'au moins 51% des capacités de calcul, il devient possible en théorie, d'outrepasser le mécanisme de consensus et donc d'imposer des blocs fallacieux qui seront ajoutés au registre officiel. 
Dès lors si un groupe devient trop puissant, il est en capacité de définir quelles informations sont légitimes au sein d'une blockchain.

{% endhint %}

##### L'exemple de la 'double dépense'

En imaginant qu'un groupe dispose de plus de 51% de la puissance totale, il peut alors procéder à une manipulation frauduleuse du registre appelée le hack de la double dépense.
 
Ce hack consiste à effectuer des transactions entre deux comptes. Il effectue un débit du premier compte vers le second, et disposant de la puissance nécessaire pour manipuler la blockchain, efface la transaction. Pour ce faire il suffit de ne pas inclure la transaction dans les blocs minés, et attendre qu'une blockchain plus longue que la blockchain courante vienne la remplacer.

Une fois la transaction effacée du registre distribué, le second compte apparait comme n'ayant jamais été débité tant que le second a bien reçu la somme.
 Il s'agit d'une création de monnaie ex-nihilo des unités de crypto-monnaie.
 
Une telle opération entraînera rapidement la chute du cours de la cryptomonnaie. Le groupe menant des activités frauduleuses devra alors rapidement convertir ses actifs dans une monnaie courante comme l'euro ou le dollar, ce qui accélèrera la chute du cours.

L'opération est facilitée par le biais de moyens automatisés.

Cette attaque est inenvisageable sur des blockchains bien installée comme le Bitcoin, en raison du coût que représente une telle opération, du moins une telle approche est inaccessible pour une entreprise privée, mais pas d'un État voyou, qui dispose des budgets nécessaires et peut avoir comme motivation de perturber une blockchain concurrente ou occasionnant un trouble.
    
À l'inverse, sur des  blockchains ayant une faible capacité de minage (récente ou de petite taille), cette attaque est facilement envisageable. 

Dans ce dernier cas, une puissance de calcul faible, dont pourrait disposer une organisation lambda suffirait à réaliser l'attaque.

{% hint style='danger' %}

Les blockchains récemment créée sont donc dans une position d'extrême vulnérabilité.

{% endhint %}

##### Les objectifs d'une attaque des 51%

* Fraude des registres et disparition des transactions:
   
   Dans le cadre d'une blockchain privée, par exemple permettant l'implémentation du vote ou permettant la traçabilité alimentaire, cela permettrait de falsifier les informations. 
   
   Dans le cas d'une cryptomonnaie, cela permet la double dépense, qui permet à la fois de s'enrichir et de déstabiliser le cours de la monnaie.

* Rompre le lien de confiance: 

    Les blockchains de par leur fonctionnement décentralisé posent des problématiques de gouvernance et sont perçues comme une menace par certains états ou institutions. C'est pourquoi perturber le fonctionnement de ces blockchains permet d'aliéner le lien de confiance des utilisateurs envers la blockchain.

##### Résilience des blockchains à l'attaque

Le système des crypto-monnaies est conçu pour être résilient aux attaques des 51%, lorsqu'une telle attaque est constatée. Un patch peut être déployé et limite les dégâts causés par l'attaque. 

###### Coûts estimés d'une attaque au 51%

Les coûts pour réaliser une attaque des 51% varie en fonction de l'échelle de la blockchain visée.

_*Concernant le Bitcoin diverses estimations ont été réalisées par Jean-Paul Delahaye dans L’attaque Goldfinger d’une blockchain.*_

À l'aide de ses calculs, on peut estimer le coût en mai 2017 à **878 millions de dollars**.

En comparaison le budget de l'État Français est de 400 milliards d'euros par an, celui d'une agence gouvernementale comme la NSA est de 45 milliards de dollars.

L'attaque est donc inaccessible à une institution lambda.

#### Stratégie du mineur égoïste
---

_*L'exemple du mineur égoïste est explicité dans Les risques des blockchains, par Laurent Dehouck, Maître de conférences en sciences de gestion, ENS Rennes et Audrey Thomas, ENSAM.*_

Lorsqu'une transaction a lieu, le mineur qui découvre la solution en premier dispose d’un bloc Be.
 
 Ce bloc est censé être communiqé aux autres nœuds afin d'être intégré dans la blockchain. 
 
 Mais ce mineur, malhonnête, peut garder ce bloc secret et travailler de suite à la validation du bloc suivant.

Dès l’instant qu'un autre mineur «honnête» valide un bloc Bh, il souhaite le diffuser aux autres nœuds. 

Le mineur malhonnête va alors diffuser son bloc Be. Le réseau se retrouve ainsi en présence de deux blocs validés presque en même temps et temporairement conservés sur la blockchain.

Certains nœuds du réseau auront connaissance du bloc Be et d’autres auront connaissances du bloc Bh. 

Des nouveaux blocs vont alors s’ajouter à la suite de Be et Bh. 

Pour le mineur malhonnête, l'avantage demeure dans l'acte de ne pas divulguer le bloc Be. Cela lui donne un avantage stratégique vis-à-vis du reste des utilisateurs du réseau pour la recherche de la solution suivante, car chaque bloc validé est relié aux blocs précédents.

La création simultanée de deux blocs provoque ce qu’on appelle une «bifurcation», dès lors la chaîne contenant sera conservée car la chaîne contenant le bloc Be sera plus longue.

Le mineur malhonnête disqualifie ses concurrents en les faisant travailler à perte, leurs rendements s'effondrant rapidement. 

 ![illustration d'une bifurcation](../../images/illustration_bifurcation.png)
 > Illustration d'une bifurcation

{% hint %}

Ce genre de stratégie invite à repenser la question de la normalisation de la blockchain et les techniques de consensus pour se prémunir contre ces pratiques délétères.

{% endhint %}
