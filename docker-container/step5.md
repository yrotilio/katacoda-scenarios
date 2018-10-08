
Objectif : comprendre le fonctionnement et l'utilisation du Dockerfile pour builder son application

## Dockerfile

`cat Dockerfile`{{execute}}

## Comprendre les options du Dockerfile

Parmis toutes les instructions d'un Dockerfile, 2 commandes sont structurelles et donc obligatoirement configurées :

* FROM : image à partir de laquelle builder l'image

* CMD : commande utilisée au lancement de l'image

* Le reste des commandes (RUN, COPY, ADD, ENV, EXPOSE, etc..) permet de configurer le contenu de l'image afin de l'instruction CMD réalise l'opération souhaitée

## Construire une page web personnalisée

`docker build -t front_web_alcyor:static .`{{execute}}

## Vérification du résultat

`docker run -d -p 8080:80 front_web_alcyor:static`{{execute}}

Tester l'accès au serveur web sur le port 8080 avec ce [lien](https://[[HOST_SUBDOMAIN]]-8080-[[KATACODA_HOST]].environments.katacoda.com/)

## Vérification du contenu de l'image

`docker inspect front_web_alcyor:static`{{execute}}

`docker history front_web_alcyor:static`{{execute}}
