By Maxime.C Alexis.O Sébastien.M

===============Installation===============
-Ne pas avoir d'autres containers de run sur les ports 80,81,443
-En cas de doute on peut éteindre tout les containers :
-----> docker-compose down
/!\ Si le projet a était installer auparavant il est préférable de supprimer les images éxistante
Pour les flemmars cette commande supprime toutes les images ;-)
-----> docker rmi $(sudo docker images -a -q)
=========================================

========Utilisation du site web=========
Le site est disponible en http : http://localhost
Le site est aussi disponible en https : https://localhost
Il est possible de s'authentifier avec un compte sur le site :
------>Username: secretaire
------>Password: secret 
- Puis il est possible de créer un compte étudiant (remplir tout les champs ) et de se connecter avec celui-ci
(Les données d'authentification provienne de la BDD mysql
========================================

=============Utilisation d'adminer================
Adminer est accessible sur : http://localhost:81
----->Username: root
----->password: root
----->server: db
----->Database: glazik
=================================================


=================Changelog=================
-Ajout de la BDD & connexion au site web
-Corrections de bugs dans le PHP du site web
-Ajout du composer pdu pdu_mysql au container php
-Création & installation du mod ssl au container nginx
==========================================

===============Bisous==================== 
