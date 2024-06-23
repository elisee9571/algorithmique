# algorithmique

## 1. Introduction à l'algorithmique
Définition et importance des algorithmes :
Un algorithme est une suite finie et ordonnée d'instructions permettant de résoudre un problème ou d'accomplir une tâche. Ils sont essentiels en informatique car ils fournissent les étapes précises nécessaires pour obtenir un résultat désiré.

### Histoire des algorithmes :
Les algorithmes existent depuis l'Antiquité, avec des exemples notables comme l'algorithme d'Euclide pour le calcul du plus grand commun diviseur. Au fil des siècles, les algorithmes ont évolué et sont devenus un pilier de l'informatique moderne.

### Algorithmes et programmation :
La programmation consiste à implémenter des algorithmes dans un langage de programmation pour créer des logiciels. Un bon programmeur doit savoir concevoir des algorithmes efficaces et les traduire en code.

## 2. Notions de base
### Variables, Constantes et types de données :
- Les variables sont des espaces mémoire qui associent un identifiant à une valeur qui peuvent varier.
- Les constantes : Contrairement à une variable, une constante est un identificateur associé à une valeur fixe.
- Les types de données courants incluent les entiers, les flottants, les caractères et les booléens.
```
a = 10;      # Nom (identifiant): a, Type: entier (integer), Valeur: 10
b = 3.14;    # Nom (identifiant): b, Type: décimal (float), Valeur: 3.14
c = 'Hello'; # Nom (identifiant): c, Type: chaîne de caractères (string), Valeur: 'Hello'
d = True     # Nom (identifiant): d, Type: booléen (boolean), Valeur: True
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
a > b;  # superieur à
a < b;  # inferieur à

# Opérations logiques
a && b; # AND
a || b; # OR
```

### Structures de contrôle :
Les structures de contrôle permettent de diriger le flux d'exécution d'un programme. 

- **Les structures conditionnelles :** (if, else) permettent d'exécuter des blocs de code selon des conditions.
```
# Stuctures conditionnelles
si condition alors
    instructions
sinon
    instructions_alternatives
```

- **Les boucles :** (for, while) permettent de répéter des blocs de code.
```
# Boucles for
pour variable de début à fin faire
    instructions

# Boucles While
tant que condition faire
    instructions
```

## 3. Conception d'algorithmes
### [pseudo-code](https://fr.wikipedia.org/wiki/Pseudo-code) et [diagrammes de flux](https://en.wikipedia.org/wiki/Flowchart) :
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
**[diagrammes de flux](https://en.wikipedia.org/wiki/Flowchart) :**


![image](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d1/For_loop_example.svg/340px-For_loop_example.svg.png)
![image](https://upload.wikimedia.org/wikipedia/commons/thumb/9/91/LampFlowchart.svg/440px-LampFlowchart.svg.png)

### Techniques de conception :
- **[Diviser pour régner](https://fr.wikipedia.org/wiki/Diviser_pour_r%C3%A9gner_(informatique)) :** Diviser le problème en sous-problèmes plus petits, les résoudre indépendamment, puis combiner leurs solutions.

- **[Recursivité](https://fr.wikipedia.org/wiki/R%C3%A9cursivit%C3%A9) :** Une fonction qui s'appelle elle-même pour résoudre des sous-problèmes identiques mais plus petits.

- **[Programmation dynamique](https://fr.wikipedia.org/wiki/Programmation_dynamique) :** Résoudre des sous-problèmes et stocker leurs solutions pour éviter des calculs redondants.

### Analyse de complexité :
L'analyse de complexité est une branche de l'informatique théorique qui étudie les ressources nécessaires à l'exécution d'algorithmes. Elle se concentre principalement sur deux types de ressources :

- **Le temps :** le nombre d'opérations nécessaires pour exécuter l'algorithme en fonction de la taille de l'entrée. On parle de complexité temporelle.

- **L'espace :** la quantité de mémoire requise par l'algorithme en fonction de la taille de l'entrée. On parle de complexité spatiale.

#### Complexité temporelle :
La complexité temporelle évalue le nombre d'étapes nécessaires pour qu'un algorithme termine son exécution. On utilise souvent la notation asymptotique pour décrire cette complexité :

- **O(n) :** La complexité linéaire. Le temps d'exécution augmente linéairement avec la taille de l'entrée.
- **O(n²) :** La complexité quadratique. Le temps d'exécution augmente proportionnellement au carré de la taille de l'entrée.
- **O(log n) :** La complexité logarithmique. Le temps d'exécution augmente logarithmiquement avec la taille de l'entrée.
- **O(n log n) :** La complexité quasi-linéaire. Couramment rencontrée dans les algorithmes de tri efficaces comme le tri par fusion.
- **O(1) :** La complexité constante. Le temps d'exécution ne dépend pas de la taille de l'entrée.

#### Complexité spatiale :
La complexité spatiale mesure la quantité de mémoire supplémentaire nécessaire à l'exécution de l'algorithme. Elle est aussi décrite en termes de notation asymptotique :

- **O(1) :** La mémoire utilisée est constante, peu importe la taille de l'entrée.
- **O(n) :** La mémoire utilisée est proportionnelle à la taille de l'entrée.
- **O(n²) :** La mémoire utilisée augmente proportionnellement au carré de la taille de l'entrée.

#### Importance de l'Analyse de Complexité :
L'analyse de complexité est cruciale pour évaluer l'efficacité des algorithmes, notamment lorsqu'ils sont appliqués à de grands ensembles de données. Elle permet de prévoir les performances et d'optimiser les choix d'algorithmes en fonction des contraintes de ressources disponibles.

## 4. Structures de données
Une structure de données est une manière d'organiser les données pour les traiter plus facilement.

### Tableaux et listes :

- **[Tableau](https://fr.wikipedia.org/wiki/Tableau_(structure_de_donn%C3%A9es)) :** Structures de données séquentielles avec une taille fixe. Accès rapide aux éléments mais insertion et suppression coûteuses.


- **[Liste](https://fr.wikipedia.org/wiki/Liste_(informatique)) :** Structures de données linéaires avec une taille dynamique. Insertion et suppression rapides mais accès plus lent.

### Piles et files :

- **Piles (LIFO - Last In, First Out) :** Dernier arrivé, premier sorti. Utilisées dans des applications comme l'évaluation d'expressions, la gestion d'undo(annuler)/redo(refaire) dans des éditeurs de texte, etc.

- **Files (FIFO - First In, First Out)  :** Premier arrivé, premier sorti. Utilisées dans des applications comme la gestion des tâches, la simulation de files d'attente, etc.

### Arbres et graphes :

- **Arbres :** Structures hiérarchiques avec un nœud racine et des nœuds enfants. Utilisés dans des algorithmes de recherche et des structures de données comme les arbres binaires de recherche.

- **Graphes :** Collections de nœuds connectés par des arêtes. Utilisés dans des algorithmes de réseaux et de parcours.

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
