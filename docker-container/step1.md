
Objectif : comprendre le fonctionnement et l'utilisation des commandes docker dans leur ensemble, et leur intéraction avec le système

# Liste des commandes docker

`docker`{{execute}}

> Seules **10** de ces commandes seront utilisées dans **95 %** des cas

## Pour les containers - aka le RUN

* `run` : instancie un container à partir d'une image docker (pullée automatiquement si elle n'existe pas en local)
* `ps` : affiche les containers locaux
* `stop`/`kill` : arrête "gracieusement"/"brutalement" un container
* `logs` : affiche les logs de la sortie standard d'un container
* `exec` : exécute une commande dans un container

## Pour les images - aka le BUILD

* `pull` : récupére une image docker en local à partir d'un registry
* `images` : affiche les images locales
* `build` : construit une image à partir d'un Dockerfile
* `push` : envoie une image docker locale vers un registry

## Pour le système - aka le RUN INFRA

* `info` : affiche les informations système du daemon docker

`docker info`{{execute}}
