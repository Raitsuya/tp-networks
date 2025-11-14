Créer 3 conteneurs sur 2 réseaux différents :

•	app et db dans backend\_net

•	proxy dans frontend\_net et backend\_net (il fait le lien entre les deux)

Exercice bonus :
Empêcher db d’être accessible directement depuis l’hôte, mais rendre l’application joignable via le proxy.



j'ai modifié le fichier compose.yml j'ai ajouté le service mariadb et le service

