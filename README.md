# Itescia Projet Docker
> Le projet est composé de trois containers, nginx, php et mysql,Il y a un site Auto-école qui s'appel Glazik d'héberger dessus avec une base de donnée Mysql permettant de se connecter sur le site mais aussi de créer des utilisateurs.

## Installation

Linux :

> Eteindre les containers actuellement run, il faut rendre disponible les ports 80,81,443,444

```sh
sudo docker-compose down
```
> Supprimer toute les images associer a une précédente version du projet, si vous souhaitez directement tout supprimer vous pouvez utiliser :

```sh
sudo docker rmi $(sudo docker images -a -q)
```

Windows:
> Pour windows il suffie d'utiliser les même commandes ci-dessus sans le sudo.

## Exemples d'usages avec le site web

Le site est disponible en https : https://localhost
Il est possible de s'authentifier avec un compte sur le site :
* Username: secretaire
* Password: secret
- Puis il est possible de créer un compte étudiant (remplir tout les champs ) et de se connecter avec celui-ci.

## Exemple d'usages avec le site de rencontre

Le site est disponible en https sur le port 444 : https://localhost:444

## Exemple d'usages avec glpi

Le site est disponible en http sur le port 81 : http://localhost:81
* Login: glpi
* Password: glpi

## Exemples d'usages avec Adminer

> Vous pouvez vérifier la présence de l'utilisateur créer sur le site web.

Adminer est accessible sur : http://localhost
* Username: root
* password: root
* server: db
* Database: glazik

## Release History
* 0.2.3
    * MODIFY Modification de love-life
    * ADD Ajout du container GLPI & creation de la bd glpidb
* 0.2.2
    * ADD: Ajout d'un Vhost love-life en mod ssl
    * MODIFY : port 80 pour Adminer
* 0.2.1
    * ADD: Création & installation du mod ssl au container nginx
* 0.2.0
    * Change: Corrections de bugs dans le PHP du site web
* 0.1.1
    * Change: Ajout du composer pdu pdu_mysql au container php
* 0.1.0
    * ADD: Ajout de la BDD & connexion au site web
* 0.0.1
    * Déploiement & configuration

## Contributeurs
* M3-Res-M1 Itescia

* Maxime.C
* Alexis.O
* Sébastien.M

