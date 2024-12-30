# Arithmétique

### Divisibilité, définition

Soient A et B deux entiers. B divise A s'il existe un entier Q tel que : A égal B fois Q. A est alors un multiple de B.


### Divisibilité, propriétés

La divisibilité est transitive.

Si A divise B et B divise A, alors A et B sont égaux ou opposés.

Si C divise A et B, alors pour tous les entiers relatifs U et V, C divise A U plus B V.


### Théorème de la division euclidienne

Soient A et B deux entiers relatifs, avec B non nul. Il existe deux entiers Q et R tels que : A égal B fois Q plus R, R étant supérieur ou égal à zéro et inférieur à la valeur absolue de B.


### Définition du PGCD

Définition du PGCD

Soient a et b deux entiers relatifs non tous les deux nuls. Le plus grand diviseur commun est le plus grand entier naturel qui divise à la fois a et b.


### Lemme d'Euclide

Lemme d'Euclide

Le plus grand diviseur commun de deux nombres est égal au plus grand diviseur commun  du plus petit d'entre eux, et du reste de la division euclidienne du plus grand par le plus petit.


### Algorithme d'Euclide

Algorithme d'Euclide pour déterminer le PGCD de deux nombres

On divise le plus grand nombre par le plus petit. Tant que le reste n'est pas nul, on divise le diviseur de la division précédente par son reste. Le PGCD est le dernier reste non nul.


### Nombres premiers entre eux

Deux nombres sont premiers entre eux si leur PGCD vaut 1.

Plusieurs nombres sont premiers dans leur ensemble si leur PGCD vaut 1.

Plusieurs nombres peuvent être premiers dans leur ensemble sans être premiers deux à deux.

Plusieurs premiers deux à deux sont aussi premiers dans leur ensemble.


### Théorème de Bézout

Quels que soient A et B entiers, il existe deux entiers U et V tels que : A fois U plus B fois V égal le PGCD de A et de B. U et V sont appelés coefficients de Bézout.


### Déterminer les coefficients de Bézout

Obtenir des coefficients de Bézout après avoir utilisé l'algorithme d'Euclide

On part de l'expression principale obtenue : en exprimant le PGCD en fonction des autres termes de la division dont il est le reste.

Puis, on remonte les lignes de l'algorithme d'Euclide, et pour chacune d'entre elles : On isole le reste à gauche. On le substitue dans l'expression principale par les termes à droite. On développe l'expression principale, en conservant les termes qui apparaissent plus haut dans les lignes de l'algorithme.

Quand on a atteint la ligne en haut, des coefficients de Bézout apparaissent.


### Corollaires du théorème de Bézout

On travaille sur l'ensemble des entiers relatifs.

Selon le théorème de Bézout, pour tout entiers *a* et *b*, on peut trouver *u* et *v* tels que *a* *u* plus *b* *v* égal le PGCD de *a* et *b*.

Si *a* et *b* sont premiers entre eux, alors il existe *u* et *v* tels que *a* *u* plus *b* *v* égal 1.

Si l'on peut trouver *u* et *v* tels que *a* *u* plus *b* *v* égal 1, alors le PGCD de *a* et *b* vaut 1.

Si *d* divise *a* et *d* divise *b*, alors *d* divise le PGCD de *a* et *b*.

Si *a* divise *b* fois *c*, et le PGCD de *a* et *b* vaut 1, alors *a* divise *c*.


### Définition PPCM

Le plus petit multiplicateur commun (PPCM) de deux nombres est le plus petit entier positif divisible par chacun d'eux.


### Propositions concernant le PPCM

Soient deux entiers.

D'une part, leur PGCD multiplié par leur PPCM est égal à la valeur absolue de leur produit.

Et d'autre part, leur PPCM divise tous leurs multiples communs.


### Définition des nombres premiers

Un nombre premier est un entier supérieur ou égal à 2, dont les seuls diviseurs positifs sont 1 et lui-même.


### Propositions sur les nombres premiers

Propositions admises

Tout entier N supérieur ou égal à 2 admet un diviseur qui est un nombre premier.

Il existe une infinité de nombre premiers.


### Déterminer si un nombre est premier

Pour déterminer si un nombre est premier, on teste sa divisibilité.

Cependant, s'il n'est pas premier, il admet un diviseur inférieur à sa racine.

On teste donc sa divisibilité : uniquement par les nombres inférieurs à sa racine, et uniquement par les nombres premiers.


### Crible d’Ératosthène

Pour déterminer quels sont les premiers nombres premiers, crible Ératosthène on peut utiliser le crible d’Ératosthène.

On écrit les nombres que l'on souhaite tester. Puis on les parcours, à partir de 2, et jusqu'à la racine carrée du plus grand nombre considéré. Le premier nombre non barré rencontré est premier. On barre tous ses multiples (à sa droite), puis on continue le parcours.


### Lemme d'Euclide

Autre lemme d'Euclide

Si P divise A fois B, et P est premier, alors P divise A ou P divise B.


### Théorème de la division en facteurs premiers

Théorème

Soit N un entier supérieur ou égal à deux. Il existe des nombres premiers et des exposants entiers tels que : N puisse être exprimé par un produit de nombre premiers à la puissance des exposants. décomposition Et cette décomposition est unique.


### Décomposition d'un entier en nombres premiers

Pour décomposer un entier en nombres premiers, on commence par 2, et on parcours les nombres premiers croissants. Pour chacun, on divise par lui le nombre à décomposer autant de fois que possible. On garde ce qu'il reste. Si ça vaut 1, la décomposition est terminée. Sinon, on passe au nombre premier suivant.


### PPCM et PGCD depuis décomposition en puissances de premiers

A partir de leur décomposition en puissances de nombres premiers, on peut calculer le PGCD de plusieurs nombres. Pour ce faire, pour chaque nombre premier, on sélectionne la puissance minimale dans chaque décomposition, et on en fait le produit.

On procède de même pour le PPCM en sélectionnant par puissance maximale.


### Indicatrice d'Euler

L'indicatrice d'Euler s'applique à : un entier naturel non nul *N*.

Elle est définie par : le nombre d'entiers strictement positifs inférieurs à *N*, dont le PGCD avec *N* vaut un.

Un cas particulier est celui *N* où est le produit de : deux nombres premiers distincts *p* et *q*.

L'indicatrice d'Euler vaut alors : *p* moins un fois *q* moins un.


#### Transcript

Soit n ∈ ℕ*, phi(n) = #{n >= j >=1 : PGCD(j, n) = 1}

Si P et Q premiers et distincts, phi(p x q) = (p - 1) * (q - 1)


### Congruences, définitions

Soient *n* un entier supérieur ou égal à 2, ainsi que *a* et *b* deux entiers relatifs.

*a* est congru à *b* modulo *n* si et seulement si :
*n | b-a**∃k∈ℤ : a=b+k \times n**a* et *b* ont le même reste de division euclidienne par leur modulo.


### Congruences, propositions

Dans la division euclidienne, le dividende est congru au reste modulo le diviseur.

La congruence est une relation d'équivalence.

La congruence modulo N partitionne les entiers relatifs en N classes d'équivalences.


### Congruences, operations

Quand on travaille modulo N, on peut réduire un nombre en lui retirant K fois N, où K est un entier naturel.

Quand on doit calculer un nombre avec exposant modulo N, on peut parfois, de cette façon, le réduire à 1 ou -1. Sinon, on peut le calculer par exposant croissants pour aboutir à 1 ou -1.

https://www.youtube.com/watch?v=SdKhHF9v9zo

7min12


### Congruences, propriétés

Si A est congru à B modulo N et C est congru à D modulo N, on a alors...

A plus C est congru à B plus D modulo N.

A fois C est congru à B fois D modulo N.

A puissance K est congru à B puissance K modulo N, où K est un entier supérieur à 0.


### Petit théorène de Fermat

Quels éléments le petit théorème de Fermat met-il en relation ? *p* un nombre premier et *a* un entier naturel non nul.

Qu'énonce-t-il ? *a* puissance *p* est congru à *a* modulo *p*.


### Inversibilité et diviseurs de zéro

Dans l'ensemble *Z* sur *k* *Z* et pour la multiplication...

L'élément neutre est un.

Concernant l'inversibilité, un élément est soit inversible, soit un diviseur de zéro.

Un nombre est inversible s'il existe un autre élément tel que leur produit égal à un.

Un nombre est un diviseur de zéro s'il existe un autre élément tel que leur produit égal à zéro.

Un nombre est inversible si et seulement si son PGCD avec *k* égal un.

Un élément est un diviseur de zéro si et seulement si son PGCD avec *k* est différent de un.


# RSA

### RSA, Principe

Le cryptage RSA consiste à découper les données en nombres et à les transformer en d'autres nombres sans relation apparente.

Le décryptage est l'opération inverse.


### RSA, Préparation

Préparation des éléments nécessaire pour RSA

On choisi *p* et *q* qui sont... des entiers premiers, distincts et de grande taille.

On calcule le module de chiffrement *N*, qui est égal à... *p* fois *q*.

On choisi *e*, l'exposant de chiffrement qui est... supérieur à 1, inférieur à phi de *N*, et premier avec phi de *N*.

Cette dernière propriété le rend... inversible dans ℤ sur phi de *N* ℤ.

On calcule *d*, l'exposant de déchiffrement qui est... l'inverse multiplicatif de *e* modulo phi de *N*.

Pour ce faire...
on applique l'algorithme d'Euclide étendu à phi de *N* et *e*.on obtient 1 égal k fois phi de *N* plus *d* fois *e*.on peut supprimer *k* fois phi de *N* car on travaille modulo phi de *N*.on obtient donc *e* fois *d* égal 1.on extrait *d* et on le ramène modulo phi de *N*.


### RSA, Encryptage

Pour encrypter un nombre par RSA, celui ci doit être... supérieur ou égale à zéro et inférieur ou égal à *N*.

L'encryptage consiste à... l'élever à la puissance *e* et appliquer modulo *N*.


### RSA, Décryptage

Pour décrypter un nombre encrypté en RSA... on l'élève à la puissance *d* et on applique modulo *N*.

### Équations diophantiennes

Les équations diophantiennes sont de la forme : A fois X plus B fois Y égal C, *a*x + b*y = c*, où A, B et C sont des entiers.

### Résolution des équations diophantiennes "simples"

Considérons une équation diophantienne dont les coefficients sont des nombres premiers et la constante vaut 1.

4 étapes sont nécessaires pour la résoudre.

Étape 1. On cherche une solution, par tâtonnement ou par l'algorithme d'Euclide.

Etape 2. On substitut la solution aux inconnues. On soustrait l'expression obtenue à l'équation initiale. On isoler les inconnues de part et d'autre de l'égalité.

Etape 3. Simplification par Gauss et réorganisation.

Etape 4. Vérification de la réciproque en substituant dans l'expression initiale.

Suite des exercices: https://www.youtube.com/watch?v=ZFhrpRr2GGQ

### Équations diophantiennes sans solutions

Une équation diophantienne, dont le PGCD des coefficients ne divise pas la constante, n'a pas de solutions.

### Petit théorène de Fermat

Quels éléments le petit théorème de Fermat met-il en relation ? *p* un nombre premier et *a* un entier naturel non nul.

Qu'énonce-t-il ? *a* puissance *p* est congru à *a* modulo *p*.
