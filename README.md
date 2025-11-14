Créer 3 conteneurs sur 2 réseaux différents :

•	app et db dans backend\_net

•	proxy dans frontend\_net et backend\_net (il fait le lien entre les deux)

Exercice bonus :
Empêcher db d’être accessible directement depuis l’hôte, mais rendre l’application joignable via le proxy.

**Projet**

1. Création de 3 conteneurs sur 2 réseaux différents :
    - app et db dans backend_net
    - proxy dans frontend_net


2. Pour lancer l'app avec la base de données
   
j'ai modifié le fichier compose.yml : j'ai ajouté les services db, app et proxy
J'ai édité mon DockerFile

<img width="476" height="184" alt="image" src="https://github.com/user-attachments/assets/3d30bf68-9343-43e4-b733-48ddf5defbff" />


3. Pour tester
docker compose up -d et aller sur un navigateur et entrer http://localhost

4. Pour vérifier si l'app et la base de données sont dans le réseau backend_net
  docker network inspect tp-networks_backend_net

5. Pour vérifier si le proxy est dans le réseau front_end
  docker network inspect tp-networks_backend_net





