
Objectif : comprendre le fonctionnement et l'utilisation des commandes docker associées aux containers (donc au RUN)

## docker run

* Démarrer un container _intéractif_ avec la commande `docker run`

`docker run -it httpd:alpine`{{execute}}

* Démarrer un container _daemon_ avec la commande `docker run`

`docker run --name front_web -d nginx:stable-alpine`{{execute}}

## docker ps

* Lister les containers en cours d'exécution avec `docker ps`

`docker ps`{{execute}}

## docker exec

* Lancer une commande dans un container en cours d'exécution avec `docker exec`

`docker exec -it front_web sh`{{execute}}

`docker exec front_web ls -lrt /var/log/nginx/`{{execute}}

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
