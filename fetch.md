# Explication de la méthode fetch

La méthode fetch en Javascript tu l'auras sans doute compris sert à récupérer, supprimer, mettre à jour des informations sur un serveur et plus simplement à effectuer des requetes HTTP. Le fameux CRUD.
Bien souvent nous allons nous en servir pour chercher des informations sur une API par exemple. Prenons cette [API](https://pokeapi.co/docs/v2#pokemon) Pokemon.
Nous allons pouvoir récupérer des informations sur les pokemons grâce à fetch en y mettant obligatoirement une url en argument.
  ```fetch("https://pokeapi.co/api/v2/pokemon/1")```
  
fetch étant une méthode asynchrone, elle renvoie donc une promesse lorsque la requête sera executé et que la réponse sera disponible. Nous aurons donc besoin d'un .then pour pouvoir avoir accéder à la réponse.

  ```
  fetch("https://pokeapi.co/api/v2/pokemon/1")
      .then(response => response.json())
  ```
 
 Comme peut le faire Express, fetch fourni également 3 interfaces (Request, Response, Headers). Celle qui nous intérresse le plus ici c'est le fameux Response. Dedans nous aurons donc la réponse
 à notre requête que nous pouvons formater en json pour que cela soit plus pratique à manipuler.
 Ici nous avons juste effectuer un  simple GET mais il est possible de faire un POST etc... en y ajoutant des paramétres supplémentaires après notre URL.
 Tout est très bien expliqué [ici](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch)
 
 En cas d'erreur il est possible également de pouvoir la récupérer ```.catch(error => alert("Erreur : " + error)); ```
 On ajoute un .catch après le .then et si une erreur se produit lors de la requête nous atterrissons ici.
 
 Pour prendre un cas concret, imaginons que tu as mis en ligne ton serveur. Tu as donc une API disponible publiquement et tu as une route /card/id qui permet de récupérer les informations d'une carte.
 A partir d'un autre projet tu vas pouvoir récupérer ces informations grâce à la méthode fetch.
 
```
fetch("https://ton-url/card/1")
    .then(response => response.json())
    .catch(error => alert("Erreur : " + error));
```

Ici tu auras dans response ton object card avec toutes les prorpriétés qui lui sont associées.

En espérant que mes explications t'auront aidé dans la compréhension de la méthode fetch.
