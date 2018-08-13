## Qu'est ce que la blockchain ?
---

Le terme blockchain désigne à la fois le système et la technologie sous-jacente à ce système.

La blockchain est connue majoritairement du grand public comme étant la technologie utlisée par le bitcoin.

Inventée en 2008, le bitcoin est à l'origine un prototype pour montrer qu'il était possible de faire reposer une crypto-monnaie dont le mécanisme repose sur un registre distribué et réparti entre de multiples noeuds d'un réseau.

De part leur nature intrinséquement open-source, les algorithmes de chiffrages sont un argument de plus au regard de la confiance en ce système.

**De fait, le bitcoin est la première manifestation de l’obsolescence d'une banque en l’occurrence en tant que tiers de confiance.**
 
### Les trois pilliers de la blockchain

Celle-ci est basée sur trois piliers : deux sont technologiques, à savoir la cryptographie asymétrique et les systèmes distribués, et le troisième est sociologique.

#### 1. La cryptographie,

Elle repose sur le concept de clé. 

Il existe deux types de clés :  les symmétriques et les assymmétriques. 

Les premières sont connues depuis l'antiquité et les secondes ont vues le jour dans les années 1970.

La seconde est essentielle à la technologie blockchain car elle permet de s'assurer 
de l'authenticité de l'expéditeur du message. L'expéditeur utilise sa clef privée pour coder un message que le destinataire peut décoder avec la clef publique de l'expéditeur.
 
Si la méthode du chiffrement symétrique à l'avantage d'être peu coûteuse en puissance de calcul, et de demeurer très sûre. 

> L'inconvénient est que pour chiffrer un message de n bits, il faut au préalable avoir échangé une clé de n bits avec le destinataire du message, et cela par une voie absolument sûre, sinon chiffrer devient inutile. 

> Claude Shannon, Communication theory of secrecy system

A cette méthode on préférera le chiffrement asymétrique qui permet de contourner l'obstacle de la clé commune aux parties prenantes.

En effet, dans le cadre du chiffrement asymétrique, deux clés sont présentes: 
la privée et la publique. La clef qui est choisie privée n'est jamais transmise à personne alors que la clef qui est choisie publique est transmissible sans restrictions.

Cette technique permet:

##### Le Chiffrement 
L'un des rôles de la clef publique est de permettre le chiffrement.c'est donc cette clef qu'utilisera un premier sujet pour envoyer des messages chiffrés à un second. L'autre clef — l'information secrète — sert à déchiffrer. Ainsi, le second sujet, et lui seul, peut prendre connaissance des messages du premier sujet. 

**La connaissance d'une clef ne permet pas de déduire l'autre.**

##### L'Authentification de l'origine

L'utilisation par l'un des sujet de sa clef privée sur le condensat d'un message, permettra à ce dernier de vérifier que le message provient bien de l'interlocuteur attendu et qu'il n'y a pas cas d'usurpation: 

il appliquera la clef publique que son interlocuteur lui a fourni sur le condensat (condensat chiffré avec la clef privée de l'autre sujet) et retrouve donc le condensat original du message.

Il lui suffira donc de comparer le condensat ainsi obtenu et le condensat réel du message pour savoir si son interlocuteur est bien celui qu'il prétend. 

C'est sur ce mécanisme notamment que fonctionne la signature numérique.

#### 2. La distribution

Internet se trouve être l'une des plus belles preuves de système distribué, nul besoin d'un opérateur de télécommunication unique pour que toute personne, où qu’ellese trouve dans le monde, puisse se connecter aux Internets.

#### 3. Le consensus distribué

Pour comprendre le concept de consensus distribué, l'exemple d'une opération de lutte contre des narco-trafiquants nous apparait le plus indiqué. 

Imaginons une ville en luttes contre le crime, tout particulièrement un cartel puissant. Dans le cadre d'une opération de luttre contre le traffic de drogues, toutes les forces de police de la région sont réunies pour anéantir les criminels.

Les différents organisations de police doivent toutes attaquerensemble pour profiter de l'effet de surprise. Le cas contraire ils seraient submergés et les trafiquants risqueraient de profiter de la confusion pour s'enfuir. 

Ils doivent donc se coordonner quant à la date et l’heure de l’attaque, et, ne pouvant pas se rencontrer tous, ils délèguent à certains le rôle de messager afin de limiter les allers et venues.

Malheureusement dans une ville aussi corrompue, on ne peut se fier à personne et certains policiers sont en réalité des criminels sous-couverture dont l'objectif est de déjouer l'attaque.

Par exemple, l’un d’entre eux peut dire à lamoitié des forces de polices qu’il faut attaquer à telle date et à telle heure, et à l’autremoitié qu’il faut se retirer, désunion qui ne leur permettra pas de bénéficier de l'effet de surprise et de la supériorité numérique.

Dans le cadre d'une opération de police, la garantie de la coordination provient du supérieur hierarchique qui tient lieu de tiers de confiance. 

**La grande nouveauté apportée par la blockchain est de proposer un système qui permet de se défaire de cette autorité hiérarchique.**

En substance, chaque force de policene peut envoyer qu’un seul ordre à la fois, associé à un horodatage. 

Mais, surtout, lesordres sont agglomérés les uns aux autres, puis chiffrés, formant une chaînestockée dans un « grand livre de transactions », lequel est redistribué à tousles services de polices en présence. 

Une chaine est ainsi formée, contenant un hash de tous les ordres précédents.

Ainsi, si un messager reçoit l’information "La perquisition aura lieu demain à 16h00", et qu’il décide de ne la répercuter qu’à la moitié des autres et d’envoyer un horaire différent à l’autre moitié, il changera la valeur de ce hash. 

Les autres messagers partageant l'informations avec tous les services de police en présence, il sera possible de déterminer les chaines incohérentes et d'identifier les corrompus simplement en comparant la valeur des hashs.

Ceci implique bien entendu que le nombre de messagers honnêtes soit supérieur au nombre de corrompus.

