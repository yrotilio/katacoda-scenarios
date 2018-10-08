
Objectif : comprendre le fonctionnement et l'utilisation des commandes docker associées aux containers (donc au RUN)

## docker run

* Démarrer un container _intéractif_ avec la commande `docker run`

`docker run -it nginx:stable-alpine`{{execute}}

* Démarrer un container _daemon_ avec la commande `docker run`

`docker run --name front_web -d nginx:stable-alpine`{{execute}}

## docker ps

* Lister les containers en cours d'exécution avec `docker ps`

`docker ps`{{execute}}

* Noter les différences avec un `ps`

`ps -ef`{{execute}}

## docker exec

* Lancer une commande dans un container en cours d'exécution avec `docker exec`{{execute}}

`docker exec -it front_web sh`{{copy}}

`docker exec front_web cat /var/log/messages`{{copy}}

## docker logs

* Récupérer les logs de la sortie standard d'un container avec la commande `docker logs`{{execute}}

`docker logs front_web`{{copy}}

## docker stop/kill

* Arrêter un container avec la commande `docker stop`{{execute}} (SIGTERM)
`docker stop front_web`{{execute}}

* Retrouver les containers arrêtés
`docker ps -a`{{execute}}

* Arrêter un container avec la commande `docker kill`{{execute}} (SIGKILL)
`docker kill front_web`{{execute}}

* Retrouver les containers arrêtés
`docker ps -a`{{execute}}
