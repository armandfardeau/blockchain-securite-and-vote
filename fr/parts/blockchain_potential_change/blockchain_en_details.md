## Qu'est-ce que la blockchain ?
---

Le terme blockchain désigne à la fois le système et la technologie sous-jacente à ce système.

La blockchain est connue majoritairement du grand public comme étant la technologie utilisée par le bitcoin.

Inventé en 2008, le Bitcoin est à l'origine un prototype destiné à démontrer la possibilité de créer une crypto-monnaie dont le mécanisme repose sur un registre distribué et réparti entre de multiples nœuds d'un réseau.

De part leur nature intrinsèquement open-source, les algorithmes de chiffrage sont un argument de plus au regard de la confiance en ce système.

**Si le Bitcoin a bénéficié d'une telle exposition médiatique, c'est qu'il s'agit d'une monnaie limitée en volume qui sort du référentiel courant. Mais surtout, il s'agit d'une monnaie qui remet en question le rôle des institutions bancaires et des états en tant que tiers de confiance et en tant qu'entité légitimes à émettre et à réguler la monnaie.**
 
### Les trois piliers de la blockchain

La blockchain est basée sur trois piliers: deux sont technologiques, à savoir la cryptographie asymétrique et les systèmes distribués, et le troisième est sociologique.

#### 1. La cryptographie,

Elle repose sur le concept de clé. 
Il existe deux types de clés:  les symétriques et les asymétriques. 

Les premières sont connues depuis l'antiquité et les secondes ont vu le jour dans les années 1970.

La seconde est essentielle à la technologie blockchain car elle permet de s'assurer 
de l'authenticité de l'expéditeur du message. L'expéditeur utilise sa clé privée pour coder un message que le destinataire peut décoder avec la clé publique de l'expéditeur. La méthode du chiffrement symétrique a l'avantage d'être peu coûteuse en puissance de calcul, et de demeurer très sûre. Malheureusement elle présente des limites:

> L'inconvénient est que pour chiffrer un message de n bits, il faut au préalable avoir échangé une clé de n bits avec le destinataire du message, et cela par une voie absolument sûre, sinon chiffrer devient inutile. 

> Claude Shannon, Communication theory of secrecy system

À cette méthode on préférera le chiffrement asymétrique qui permet de contourner l'obstacle de la clé commune aux parties prenantes.
En effet, dans le cadre du chiffrement asymétrique, deux clés sont présentes: 
la privée et la publique. La clé qui est choisie privée n'est jamais transmise à personne alors que la clé qui est choisie publique est transmissible sans restriction.

Cette technique permet:

* ##### Le chiffrement
 
    L'un des rôles de la clé publique est de permettre le chiffrement. C'est donc cette clé qu'utilisera un premier sujet pour envoyer des messages chiffrés à un second. L'autre clé — l'information secrète — sert à déchiffrer. Ainsi, le second sujet, et lui seul, peut prendre connaissance des messages du premier sujet. 

    **La connaissance d'une clé ne permet pas de déduire l'autre clé.**

* ##### L'Authentification de l'origine

    L'utilisation par l'un des sujets de sa clé privée sur le condensat d'un message permettra à ce dernier de vérifier que le message provient bien de l'interlocuteur attendu et de prévenir l'usurpation: 
    il appliquera la clé publique que son interlocuteur lui a fournie sur le condensat (condensat chiffré avec la clé privée de l'autre sujet) et retrouve donc le condensat original du message.
    
    Il lui suffira donc de comparer le condensat ainsi obtenu et le condensat réel du message pour savoir si son interlocuteur est bien celui qu'il prétend. C'est sur ce mécanisme notamment que fonctionne la signature numérique.

#### 2. La distribution

Internet se trouve être l'une des plus belles preuves de système distribué, nul besoin d'un opérateur de télécommunication unique pour que toute personne, où qu’elle se trouve dans le monde, puisse se connecter aux Internets.

#### 3. Le consensus distribué

Pour comprendre le concept de consensus distribué, l'exemple d'une opération de lutte contre des narco-trafiquants nous apparait le plus indiqué. 

Imaginons une ville en lutte contre le crime, tout particulièrement un cartel puissant. Dans le cadre d'une opération de lutte contre le trafic de drogue, toutes les forces de police de la région sont réunies pour anéantir les criminels.

Les différentes organisations de police doivent toutes attaquer ensemble pour profiter de l'effet de surprise. Le cas contraire elles seraient submergées et les trafiquants risqueraient de profiter de la confusion pour s'enfuir. 

Ils doivent donc se coordonner quant à la date et l’heure de l’attaque, et, ne pouvant pas se rencontrer tous, ils délèguent à certains le rôle de messager afin de limiter les allers et venues.

Malheureusement dans une ville aussi corrompue, on ne peut se fier à personne et certains policiers sont en réalité des criminels sous-couverture dont l'objectif est de déjouer l'attaque.

Par exemple, l’un d’entre eux peut dire à la moitié des forces de polices qu’il faut attaquer à telle date et à telle heure, et à l’autre moitié qu’il faut se retirer, désorganisation qui ne leur permettra pas de bénéficier de l'effet de surprise et de la supériorité numérique.

**La grande nouveauté apportée par la blockchain est de proposer un système qui permet de se défaire de cette autorité hierarchique.**

En substance, chaque force de police ne peut envoyer qu’un seul ordre à la fois, associé à un horodatage.

Mais, surtout, les ordres sont agglomérés les uns aux autres, puis chiffrés, formant une chaîne stockée dans un «grand livre de transactions», lequel est redistribué à toutes les services de polices en présence. 

Une chaîne est ainsi formée, contenant un hash de tous les ordres précédents.

Ainsi, si un messager reçoit l’information «La perquisition aura lieu demain à 16h00», et qu’il décide de ne la répercuter qu’à la moitié des autres et d’envoyer un horaire différent à l’autre moitié, il changera la valeur de ce hash.

Les autres messagers partageant l'information avec tous les services de police en présence, il sera possible de déterminer les chaînes incohérentes et d'identifier les corrompus simplement en comparant la valeur des hashs.

Ceci implique bien entendu que le nombre de messagers honnêtes soit supérieur au nombre de corrompus.

### Les différentes méthodes de consensus:

| Type de consensus | Description | Avantages | Inconvénients | Type de blockchain|
|:-----------------:|-------------|-----------|---------------|-------------------|
| Preuve de travail (PoW) | Les ordinateurs des mineurs sont mis à disposition pour résoudre un problème mathématique compliqué. Le 1er qui trouve une solution gagne la récompense du prochain bloc de la chaîne. | Sécurisé, éprouvé et robuste. | Très consommateur d’électricité et de matériel informatique. | Publique
| Preuve de l'enjeu (PoS) | Les validateurs de transactions doivent mettre en gage la possession de cryptomonnaie pour recevoir une récompense. Si un nœud est malveillant, il peut perdre sa mise en gage au profit des validateurs honnêtes. | Peu consommateur en ressources énergétiques. | Peu testé à grande échelle. | Publique |
| Système tolérant les défaillances (PBFT) | Consensus dont la liste des validateurs est connue au départ et peut tolérer jusqu’à 1/3 de nœuds compromis (déconnectés ou malveillants). | Consensus de groupe rapide et performant. Pas de fork ou de réorganisation de chaîne. | | Privée |
| Preuve d'autorité |  Consensus dont la liste des validateurs est connue au départ et qui valide à tour de rôle un bloc. Ce type de consensus peut tolérer jusqu’à 49% de nœuds malveillants ou déconnectés. | Consensus de groupe rapide. | | Privée |
