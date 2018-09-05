
Objectif : comprendre le fonctionnement et l'utilisation des commandes docker associées aux containers (donc au RUN)

## docker run

* Démarrer un container _intéractif_ avec la commande `docker run`

`docker run -it nginx:stable-alpine`{{execute}}

* Démarrer un container _daemon_ avec la commande `docker run`

`docker run -d nginx:stable-alpine`{{execute}}

## docker ps

`docker ps`{{execute}}

`ps -ef`{{execute}}

## docker exec

`docker exec`{{execute}}

## docker logs

`docker logs`{{execute}}

## docker stop/kill

`docker stop`{{execute}}

`docker ps`{{execute}}
