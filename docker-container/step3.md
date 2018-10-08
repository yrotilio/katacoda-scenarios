
Objectif : comprendre le fonctionnement et l'utilisation des options de la commande docker run

## Lister les options de la commande docker run

`docker run --help`{{execute}}

> Une nouvelle fois, peu d'options utilisées dans la plupart des cas

* `-it` : interactif
* `-d` : daemon
* `-P` : mapper tous les ports exposés par le container sur des ports aléatoires
* `-p` : déclaration explicite des ports à mapper en paramètres (format container:hôte)
* `--privileged` : container autorisé à accéder à la socker docker == droits root sur l'hôte
* `-v` : monter un volume

## Démarrer et exposer un serveur web

`docker run -d -p 80:80 nginx:stable-alpine`{{execute}}

Tester l'accès au server web sur le port 80