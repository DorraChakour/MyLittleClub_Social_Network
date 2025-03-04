# MyLittleClub - Réseau Social Limité
## Qu'est-ce que MyLittleClub ?
MyLittleClub est une application web sociale conçue pour limiter les interactions à un nombre gérable, favorisant des connexions plus profondes et de meilleure qualité. Inspiré du nombre de Dunbar, ce projet permet aux utilisateurs de maintenir des relations significatives sans être submergés.

Ce projet utilise le framework PHP CodeIgniter 4, connu pour sa rapidité, sa légèreté et sa flexibilité.

## Installation et Mise à Jour
### Installation
Pour installer le projet, suivez les étapes suivantes :

Clonez le dépôt :
bash
Copier
Modifier
git clone https://github.com/zinebfennich/MyLittleClub-.git
cd MyLittleClub-
Installez les dépendances avec Composer :
bash
Copier
Modifier
composer install
### Mise à Jour
Lorsque des mises à jour sont disponibles, exécutez la commande suivante pour maintenir le projet à jour :

bash
Copier
Modifier
composer update
Avant de mettre à jour, consultez les notes de version pour vérifier s'il y a des modifications spécifiques à apporter.

## Configuration
Copiez le fichier env en .env et personnalisez-le selon votre configuration :

Base URL : Définissez l'URL de votre application.
Base de données : Configurez vos informations de connexion MySQL.
Vérifiez les autorisations du dossier writable, utilisé par CodeIgniter pour les fichiers temporaires.

## Organisation du Projet
Pour des raisons de sécurité, le fichier index.php se trouve dans le dossier public, séparé des autres composants de l'application.

Configurez votre serveur web pour pointer directement vers le dossier public/.
Une meilleure pratique consiste à utiliser un hôte virtuel.
## Fonctionnalités Clés
Limitation à 50 relations par utilisateur pour privilégier la qualité des connexions.
Limitation à 10 publications par jour pour éviter la surcharge d'informations.
Design inspiré des réseaux sociaux comme Twitter et Reddit.
Gestion intuitive et légère grâce à CodeIgniter 4.
## Requêtes Serveur
MyLittleClub nécessite les configurations suivantes :

PHP version 7.4 ou supérieure (recommandé : PHP 8.1 ou plus récent).
Extensions PHP nécessaires :
intl
mbstring
json (activé par défaut)
mysqlnd (si MySQL est utilisé)
libcurl (si vous utilisez HTTP\CURLRequest)
⚠️ Attention : PHP 7.4 est arrivé en fin de vie en novembre 2022. PHP 8.0 est également arrivé en fin de vie en novembre 2023. Assurez-vous d'utiliser une version prise en charge, comme PHP 8.1 ou ultérieure.

## Contribution
Pour signaler des problèmes ou proposer des idées :

Utilisez les issues GitHub de ce dépôt pour les bogues et les suggestions.
Discutez des nouvelles fonctionnalités via des demandes ou sur le forum associé.
## Ressources Utiles
CodeIgniter Documentation : CodeIgniter User Guide.
Dépôt Principal : Suivez les mises à jour et les fonctionnalités sur le dépôt principal de CodeIgniter.
