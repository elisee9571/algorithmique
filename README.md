# algorithmique

## 1. Introduction à l'algorithmique
Définition et importance des algorithmes :
Un algorithme est une suite finie et ordonnée d'instructions permettant de résoudre un problème ou d'accomplir une tâche. Ils sont essentiels en informatique car ils fournissent les étapes précises nécessaires pour obtenir un résultat désiré.

### Histoire des algorithmes :
Les algorithmes existent depuis l'Antiquité, avec des exemples notables comme l'algorithme d'Euclide pour le calcul du plus grand commun diviseur. Au fil des siècles, les algorithmes ont évolué et sont devenus un pilier de l'informatique moderne.

### Algorithmes et programmation :
La programmation consiste à implémenter des algorithmes dans un langage de programmation pour créer des logiciels. Un bon programmeur doit savoir concevoir des algorithmes efficaces et les traduire en code.

## 2. Notions de base
### Variables et types de données :
Les variables sont des emplacements de mémoire pour stocker des données. Les types de données courants incluent les entiers, les flottants, les caractères et les booléens.
```
a = 10; # integer (entier)
b = 3.14; # float (decimal)
c = 'Hello'; # string (chaîne de caractères)
d = True # boolean
```

### Opérations de base :
Les opérations incluent les opérations arithmétiques (addition, soustraction, multiplication, division), les opérations de comparaison (égal à, different de, supérieur à, inférieur à) et les opérations logiques (et, ou).
```
# Opérations arithmétiques
a + b; # addition
a - b; # soustraction
a * b; # multiplication
a / b; # division

# Opérations de comparaisons
a == b; # egal à
a != b; # different de
a > b; # superieur à
a < b; # inferieur à

# Opérations logiques
a && b; # AND
a || b; # OR
```

### Structures de contrôle :
Les structures de contrôle permettent de diriger le flux d'exécution d'un programme. 

- **Les structures conditionnelles :**
(if, else) permettent d'exécuter des blocs de code selon des conditions.
```
# Stuctures conditionnelles
si condition alors
    instructions
sinon
    instructions_alternatives
```

- **Les boucles :**
(for, while) permettent de répéter des blocs de code.
```
# Boucles for
pour variable de début à fin faire
    instructions

# Boucles While
tant que condition faire
    instructions
```

## 3. Conception d'algorithmes
### Pseudocode et diagrammes de flux :
Le pseudocode est une description textuelle des algorithmes utilisant un langage informel. Les diagrammes de flux représentent graphiquement les étapes d'un algorithme.
```
# Pseudo code
Algorithme SommeNEntiers
  Entrée : Un entier n
  Sortie : La somme des entiers de 1 à n

  somme <- 0
  pour i de 1 à n faire
      somme <- somme + i
  fin pour
  retourner somme
```
**Diagramme de flux :**


![Diagramme de flux](https://github.com/elisee9571/algorithmique/blob/main/diagramme-de-flux.png)

### Techniques de conception :
- **Diviser pour régner :** 
Diviser le problème en sous-problèmes plus petits, les résoudre indépendamment, puis combiner leurs solutions.

- **Récursivité :**
Une fonction qui s'appelle elle-même pour résoudre des sous-problèmes identiques mais plus petits.

- **Programmation dynamique :**
Résoudre des sous-problèmes et stocker leurs solutions pour éviter des calculs redondants.

### Analyse de complexité :

- **Complexité temporelle :**
Temps nécessaire à l'exécution de l'algorithme (exprimé en fonction de la taille de l'entrée, comme O(n), O(log n)).

- **Complexité spatiale :**
Espace mémoire nécessaire à l'exécution de l'algorithme.

## 4. Structures de données
### Tableaux et listes :

- **Tableaux :**
Structures de données linéaires avec une taille fixe. Accès rapide aux éléments mais insertion et suppression coûteuses.

- **Listes :**
Structures de données linéaires avec une taille dynamique. Insertion et suppression rapides mais accès plus lent.

### Piles et files :

- **Piles (LIFO) :**
Dernier arrivé, premier sorti. Utilisées dans des applications comme l'évaluation d'expressions.

- **Files (FIFO) :**
Premier arrivé, premier sorti. Utilisées dans des applications comme la gestion des tâches.

### Arbres et graphes :

- **Arbres :**
Structures hiérarchiques avec un nœud racine et des nœuds enfants. Utilisés dans des algorithmes de recherche et des structures de données comme les arbres binaires de recherche.

- **Graphes :**
Collections de nœuds connectés par des arêtes. Utilisés dans des algorithmes de réseaux et de parcours.

### Tables de hachage :
Une structure de données qui mappe des clés à des valeurs pour un accès rapide. Utilisée dans des applications comme la mise en cache et les bases de données.

## 5. Algorithmes de tri et de recherche
### Algorithmes de tri :

- **Tri à bulles :**
Compare et échange les éléments adjacents.

- **Tri par insertion :**
Insère chaque élément à sa place correcte.

- **Tri rapide (Quicksort) :**
Divise pour régner, utilise un pivot pour diviser la liste.

- **Tri fusion (Mergesort) :**
Divise la liste en sous-listes, trie et fusionne.

### Algorithmes de recherche :

- **Recherche linéaire :**
Parcourt chaque élément jusqu'à trouver l'élément recherché.

- **Recherche dichotomique (binaire) :**
Divise la liste en deux à chaque étape, recherche dans la moitié appropriée.

## 6. Algorithmes de graphes
### Représentation des graphes :

- **Listes d'adjacence :**
Chaque nœud stocke une liste de ses voisins.

- **Matrices d'adjacence :**
Tableau à deux dimensions représentant les connexions.

### Parcours de graphes :

- **DFS (Depth-First Search) :**
Parcourt les nœuds en profondeur.

- **BFS (Breadth-First Search) :**
Parcourt les nœuds en largeur.

### Algorithmes de chemin minimal :

- **Dijkstra :**
Trouve le chemin le plus court à partir d'un nœud source vers tous les autres nœuds.

- **Bellman-Ford :**
Gère les graphes avec des poids négatifs.

### Algorithmes de parcours de graphes :

- **Kruskal :**
Trouve l'arbre couvrant minimum en utilisant les arêtes les moins coûteuses.

- **Prim :**
Développe l'arbre couvrant minimum à partir d'un nœud initial.

## 7. Algorithmes avancés

### Programmation dynamique :

- **Problème du sac à dos :**
Trouve la meilleure combinaison d'objets pour maximiser la valeur tout en respectant une contrainte de poids.

- **Sous-séquence commune maximale :**
Trouve la plus longue sous-séquence commune entre deux séquences.

### Backtracking :

- **Problème des N reines :**
Place N reines sur un échiquier de taille NxN sans qu'elles ne se menacent.

- **Sudoku :**
Résout le puzzle en remplissant les cases tout en respectant les contraintes.

### Calculs numériques :

- **Méthode de Newton-Raphson :**
Approximations successives pour trouver les racines d'une fonction.

- **Algorithme d'Euclide :**
Trouve le plus grand commun diviseur de deux nombres.

## 8. Algorithmes en intelligence artificielle
### Recherche informée :

- **A\* :**
A* Algorithme de recherche utilisant des heuristiques pour trouver le chemin le plus court.

- **Recherche gloutonne :**
Utilise des heuristiques pour choisir les actions les plus prometteuses à chaque étape.

### Apprentissage supervisé :

- **Régression linéaire :**
Modèle les relations entre une variable dépendante et une ou plusieurs variables indépendantes.

- **Arbres de décision :**
Modèle les décisions et leurs conséquences sous la forme d'un arbre.

### Apprentissage non supervisé :

- **K-means :**
Partitionne les données en K clusters basés sur la similarité.

- **PCA (Principal Component Analysis) :**
Réduit la dimensionnalité des données tout en conservant la variance.
