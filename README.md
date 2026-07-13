# landing-page-e-commerce

 Nom : Agrico-service[Projet 5]
 équipe*
 
 lead: Tsiba Gaevie
 
 Répo Admin:Tsiba Gaevie
 
 Développeur: Arti-service
 
 lien Github page:https://loriontsiba-debug.github.io/landing-page-e-commerce/
 
 Rapport du conflit:
 
Pour créer un conflit Git, j’ai commencé par créer une nouvelle branche à partir de la branche main avec la commande :

git checkout -b test

Ensuite, je suis revenu sur la branche principale :

git checkout main

Dans la branche main, j’ai modifié une ligne d’un 58 dans le fichier index.html, puis j’ai enregistré les modifications :

git add .
git commit -m "Modification dans la branche main"

Après cela, je suis retourné sur la branche test :

git checkout test

J’ai modifié la même ligne 58 du fichier html, mais avec un contenu différent, puis j’ai enregistré les modifications :

git add .
git commit -m "Modification dans la branche test"

Enfin, je suis revenu sur la branche main et j’ai lancé la fusion :

git checkout main
git merge test

À ce moment-là, Git a détecté que la même ligne avait été modifiée différemment dans les deux branches et a signalé un conflit de fusion.

Pour résoudre le conflit, j’ai ouvert le fichier concerné, supprimé les marqueurs de conflit (<<<<<<<, =======, >>>>>>>), choisi la version à conserver , puis j’ai enregistré le fichier.

Enfin, j’ai validé la résolution du conflit avec les commandes :

git add .
git commit -m "Résolution du conflit de fusion"

Le conflit était alors résolu et les deux branches ont pu être fusionnées.
