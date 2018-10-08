
Objectif : comprendre le fonctionnement et l'utilisation des commandes docker associées aux images (donc au BUILD)

## docker pull

* Récupérer une image Docker avec la commande `docker pull`

> Liste des images publiques disponibles sur [dockerhub](https://hub.docker.com)

`docker pull nginx:stable-alpine`{{execute}}

## docker build

* Construire une image basique la commande avec la commande  `docker build`

`docker build --help`{{execute}}

## docker images

* Lister les images docker disponibles en **local** avec la commande `docker images`

`docker images`{{execute}}

## docker push

* Pusher une image avec la commande avec la commande  `docker push` 

`docker push --help`{{execute}}

## L'espace disque des images

`docker system df`{{execute}}

`docker pull nginx:alpine && docker pull nginx && docker pull nginx:latest`{{execute}}

`docker system df`{{execute}}
