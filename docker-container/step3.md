# But

Démarrer un serveur web et l'exposer en une commande

## Comprendre les options de la commande docker run

`docker run --help`{{execute}}

> Encore une fois, peu d'options utilisées dans la plupart des cas :
> -it : interactif
> -d : daemon
> -P : mapper tous les ports exposés par le container sur des prots aléatoires
> -p : déclaration explicite des ports à mapper en paramètres (format container:hôte)
> --privileged : container autorisé à accéder à la socker docker == droits root sur l'hôte
> -v : monter un volume

## Démarrer un serveur web

`docker run -d -p 80:80 nginx:stable`{{execute}}
