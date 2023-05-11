# Feedback

George, je vois que tu as eu un peu de mal avec ce parcours. Ne t'en fais pas nous allons t'aider à comprendre certaines notions pour que tu puisses continuer à avancer :)

Pour la première étape il était demandé ici d'afficher le détail d'une carte. Ta requête est correct ainsi que ton controller c'est au niveau de ta view que cela pêche. Pourquoi utiliser un "for" ici alors que l'on souhaite afficher
uniquement les détails d'UNE seule carte? De plus dans ton controller tu envoies à ta view un argument que tu nommes "oneCard" et tu ne l'utilises pas dans ta view. Tu ne peux pas utiliser autre chose que "oneCard" dans ta view donc
utiliser "card" ne fonctionnera pas car il n'est pas déclaré (connu). 
Ensuite il aurait été préférable d'utiliser une liste pour afficher les éléments de la carte. (ul -> li ).

N'hésites pas à relire les fondamentaux que tu viens d'apprendre depuis le début de ta formation, il est important d'avoir des bases stables pour continuer à progresser.
Ensuite corrige l'étape 1 en suivant mes remarques et une fois que tu auras fais ceci tout devrait couler. Je vois que pour l'étape 2 tu as essayé quelquechose mais il y a quelques erreurs mais que tu n'as pas commises lors de la 
première étape. Aide toi de ce qui tu as réussi à faire pour les prochaines étapes. Tu as réussi à créer une route avec un paramétre, tu as réussi à requêter la base avec ce paramètre et à envoyer tout cela dans une view.
L'étape 2 ne sera qu'une formalité.
Concernant les sessions tu as bien initialisé la session il ne te reste plus qu'a ajouter et supprimer des cartes dedans grâce à des fonctions JS (push, filter etc ...)

Tu peux déja être fier de ce que tu as fait, même si le résultat attendu n'est pas parfait, les erreurs commises sont sommes toutes assez bêtes donc facile à corriger. Avec un peu de courage et de volonté tu arriveras
à finir ce parcours.
Si tu as besoin d'aide, n'hésites pas à contacter tes camarades de promo, tes professeurs ou moi même ;)
