
Objectif : comprendre le fonctionnement et l'utilisation du Dockerfile pour builder son application

## Dockerfile

`cat Dockerfile`{{execute}}

## Comprendre les options du Dockerfile

> Il existe 2 commandes structurelles pour la création d'un Dockerfile :
> FROM : 
> CMD : 
> Le reste des commandes (RUN, COPY, ADD, ENV, EXPOSE, etc..) permet de configurer

## Construire une page web personnalisée

`docker build -t monimage:tag`{{execute}}

## Vérification du résultat

`docker run -d -p 80:80 monimage:tag`{{execute}}

