MyLittleClub - Réseau Social Limité
Qu'est-ce que MyLittleClub ?
MyLittleClub est une plateforme sociale conçue pour limiter le nombre d'interactions entre ses utilisateurs, afin de favoriser des relations plus profondes et de meilleure qualité. S'inspirant du nombre de Dunbar, ce projet permet aux utilisateurs de maintenir des connexions significatives sans être submergés par trop de sollicitations.

Cette application utilise le framework PHP CodeIgniter 4, apprécié pour sa rapidité, sa légèreté et sa flexibilité.

Installation et Mise à Jour
Installation
Pour installer le projet sur votre machine, suivez les étapes ci-dessous :

Clonez le dépôt avec la commande suivante :

bash
Copier
Modifier
git clone https://github.com/zinebfennich/MyLittleClub-.git
cd MyLittleClub-
Installez les dépendances avec Composer :

bash
Copier
Modifier
composer install
Mise à Jour
Lorsque des mises à jour sont disponibles, exécutez la commande suivante pour mettre le projet à jour :

bash
Copier
Modifier
composer update
Avant toute mise à jour, consultez les notes de version pour vérifier s'il y a des ajustements à effectuer.

Configuration
Copiez le fichier env en .env et personnalisez-le en fonction de votre environnement. Les paramètres à configurer sont les suivants :

Base URL : Définissez l'URL de votre application.
Base de données : Configurez les informations de connexion à votre base de données MySQL.
Vérifiez les autorisations du dossier writable, utilisé par CodeIgniter pour les fichiers temporaires.
Organisation du Projet
Le fichier index.php est placé dans le dossier public pour des raisons de sécurité, séparé des autres composants de l'application.

Configurez votre serveur web pour qu'il pointe directement vers le dossier public/. Il est recommandé de configurer un hôte virtuel pour cette configuration.

Fonctionnalités Principales
Limitation à 50 relations par utilisateur pour garantir des connexions de qualité.
Limitation à 10 publications par jour afin d'éviter une surcharge d'informations.
Design inspiré des réseaux sociaux comme Twitter et Reddit.
Gestion intuitive et légère grâce à l'utilisation de CodeIgniter 4.
Exigences Serveur
Pour exécuter MyLittleClub, votre serveur doit répondre aux exigences suivantes :

PHP 7.4 ou supérieur (recommandé : PHP 8.1 ou plus récent).
Extensions PHP nécessaires :
intl
mbstring
json (activé par défaut)
mysqlnd (si vous utilisez MySQL)
libcurl (si vous utilisez la bibliothèque HTTP\CURLRequest)
⚠️ Avertissement : PHP 7.4 a atteint sa fin de vie en novembre 2022, et PHP 8.0 a atteint sa fin de vie en novembre 2023. Il est recommandé de passer à PHP 8.1 ou supérieur.

Contribution
Pour signaler des problèmes ou suggérer des améliorations :

Utilisez les issues sur GitHub pour les bogues et suggestions.
Discutez des nouvelles fonctionnalités via des demandes de pull ou sur le forum associé.
Ressources Utiles
Documentation CodeIgniter : CodeIgniter User Guide
Dépôt Principal CodeIgniter : Suivez les mises à jour et les nouvelles fonctionnalités sur le dépôt officiel de CodeIgniter.
CodeIgniter 4 Application Starter
Qu'est-ce que CodeIgniter ?
CodeIgniter est un framework PHP full-stack léger, rapide, flexible et sécurisé.
Plus d'informations sont disponibles sur le site officiel.

Ce dépôt contient un starter app que vous pouvez installer avec Composer. Il a été construit à partir du dépôt de développement de CodeIgniter 4.

Pour plus d'informations sur les plans de la version 4, consultez CodeIgniter 4 sur les forums.

Vous pouvez également consulter le guide de l'utilisateur correspondant à la version la plus récente du framework.

Installation & mises à jour
Installez le projet avec Composer :

bash
Copier
Modifier
composer create-project codeigniter4/appstarter
Mettez à jour le projet en exécutant :

bash
Copier
Modifier
composer update
Lors de chaque mise à jour, vérifiez les notes de version pour voir s'il y a des changements à appliquer à votre dossier app. Les fichiers affectés peuvent être copiés ou fusionnés depuis vendor/codeigniter4/framework/app.

Configuration
Copiez env en .env et personnalisez-le pour votre application, notamment l'URL de base et les paramètres de base de données.

Changements importants concernant index.php
Le fichier index.php n'est plus à la racine du projet, il a été déplacé dans le dossier public pour améliorer la sécurité et séparer les composants.

Cela signifie que vous devez configurer votre serveur web pour pointer directement vers le dossier public/, et non pas vers la racine du projet. Une bonne pratique consiste à configurer un hôte virtuel pointant vers ce dossier.

Veuillez consulter le guide de l'utilisateur pour une meilleure explication de la manière dont CI4 fonctionne !

Gestion du dépôt
Nous utilisons les issues de GitHub dans notre dépôt principal pour suivre les BUGS et les DEVELOPPEMENT des packages approuvés.
Pour plus de soutien, utilisez notre forum et discutez des demandes de fonctionnalités.

Ce dépôt est un "dépôt de distribution", construit par notre script de préparation des versions. Les problèmes rencontrés peuvent être remontés sur notre forum ou dans les issues du dépôt principal.

Exigences Serveur
PHP version 7.4 ou supérieure est nécessaire, avec les extensions suivantes installées :

intl
mbstring
⚠️ Avertissement : PHP 7.4 a atteint sa fin de vie en novembre 2022. PHP 8.0 a atteint sa fin de vie en novembre 2023. Si vous utilisez encore PHP 7.4 ou 8.0, il est fortement conseillé de passer à une version plus récente. PHP 8.1 arrivera en fin de vie en novembre 2024.

De plus, assurez-vous que les extensions suivantes sont activées :

json (activé par défaut - ne le désactivez pas)
mysqlnd si vous prévoyez d'utiliser MySQL
libcurl si vous prévoyez d'utiliser la bibliothèque HTTP\CURLRequest
