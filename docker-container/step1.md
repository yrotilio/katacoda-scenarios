# But

Comprendre le fonctionnement du binaire docker

## docker

Lister les commandes *Docker* avec la commande `docker`{{execute}}

> Seules 10 de ces commandes seront utilisées dans 95 % des cas :
> * Pour les containers
> run : instancie un container à partir d'une image docker (pullée automatiquement si elle n'existe pas en local)
> ps : affiche les containers locaux
> stop/kill : arrête "gracieusement"/"brutalement" un container
> logs : affiche les logs de la sortie standard d'un container
> exec : exécute une commande dans un container
> * Pour les images
> pull : récupére une image docker en local à partir d'un registry
> images : affiche les images locales
> build : construit une image à partir d'un Dockerfile
> push : envoie une image docker locale vers un registry
