# Correction MCD

Dans l'ensemble tu as bien compris l'exercice et ton MCD est plutôt correct.

En effet il n'y a que les cardinalités entre USER et PRODUCT qui pose problème. Dans l'énoncé il est bien dit qu'un utilisateur peut liker un ou plusieurs produits.
Ici nous aurons donc une relation de type Many to Many.

Il faut donc y mettre 1,N du côté USER car un utilisateur peut liker un ou plusieurs produits et 0,N du côté
 PRODUCT car un produit peut être liker par aucun ou plusieurs utilisateurs.

Nous pouvons aussi discuter de la cardinalité entre ADDRESS et USER car une adresse pourrait potentiellement appartenir à un ou plusieurs utilisateurs (plusieurs
 compte dans un même foyer).
 
Pour t'aider dans la conception de MCD tu peux utiliser des outils en ligne comme par exemple [Mocodo](https://www.mocodo.net) ou alors [Diagram.net](https://app.diagrams.net)
