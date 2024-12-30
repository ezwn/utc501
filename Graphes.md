# Graphes

## Définition

Quel sont les deux ensembles qui définissent un graphe ? Premièrement l'ensemble de ses sommets, et deuxièmement ensemble de ses arrêtes.

## Graphes particuliers

Comment qualifie-t-on un graphe, dont tous les sommets sont reliés directement ou indirectement ? On dit qu'il est "connexe".

Comment appeler un graphe, dont tous les sommets sont reliés directement ? C'est un graphe "complet".

## Chemin

Dans un graphe non orienté, un chemin est une suite d'arêtes consécutives, qui n'emprunte qu'une fois chaque arête.

Un chemin simple est un chemin qui ne passe qu'une fois par sommet.


## Circuit

Dans un graphe, un circuit est un chemin qui commence et termine par le même point.


## Cycle

Dans un graphe, qu'est ce qu'un cycle ? C'est un chemin d'un sommet à lui-même, qui ne repasse pas deux fois par le même sommet.


## Arbre

Quelles sont des deux caractéristiques du graphe d'un arbre ? Il est connexe et il est acyclique.

Si *s* est son nombre de sommets, combien un arbre a-t-il d'arêtes ? *s* mois 1.


## Matrice d'adjacence

Dans la matrice d'adjacence d'un graphe, les lignes et les colonnes correspondent aux sommets du graphe.

Chaque coefficient vaut, soit 1 si les sommets sont liés par une arête, soit 0.

Dans le cas d'un graphe non orienté, cette matrice est symétrique.

En élevant cette matrice à la puissance *n*, on obtient le nombre de trajets de taille *n* permettant d'aller d'un sommet à un autre.


## Degré des sommets

Dans un graphe non orienté, le degré d'un sommet est le nombre d'arêtes qui lui sont connectées.

La somme des degrés correspond alors au double du nombre des arêtes.

Et le nombre de sommets de degré impair est pair.


## Eulérien

Eulérien signifie "qui passe une et une seule fois par chaque arrête du graphe".

Un circuit est eulérien si et seulement si le graphe est non orienté et connexe, et les degrés de tous ses sommets sont pairs.

