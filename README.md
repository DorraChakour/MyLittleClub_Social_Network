# MyLittleClub - Réseau Social Limité

## Qu'est-ce que MyLittleClub ?

MyLittleClub est une plateforme web sociale pensée pour restreindre les interactions à un nombre gérable, favorisant des connexions plus profondes et de meilleure qualité. S'inspirant du nombre de Dunbar, ce projet permet aux utilisateurs de maintenir des relations significatives sans se retrouver submergés par une multitude de connexions superficielles.

Ce projet repose sur le framework PHP CodeIgniter 4, qui est réputé pour sa rapidité, sa légèreté et sa flexibilité.

## Installation et Mise à Jour

### Installation

Pour installer le projet, suivez ces étapes :

1. Clonez le dépôt :  
   `git clone https://github.com/zinebfennich/MyLittleClub-.git`  
   `cd MyLittleClub-`

2. Installez les dépendances avec Composer :  
   `composer install`

### Mise à Jour

Lorsque des mises à jour sont disponibles, exécutez la commande suivante pour garder votre projet à jour :

   `composer update`

Avant de procéder à la mise à jour, consultez les notes de version pour vous assurer qu'il n'y a pas de modifications spécifiques à appliquer.

## Configuration

1. Copiez le fichier `env` en `.env` et adaptez-le selon votre configuration.
   
2. Personnalisez les paramètres suivants :  
   - **Base URL** : Définissez l'URL de votre application.  
   - **Base de données** : Configurez vos informations de connexion MySQL.  
   - **Permissions** : Vérifiez les autorisations du dossier `writable`, utilisé par CodeIgniter pour les fichiers temporaires.

## Organisation du Projet

Le fichier `index.php` est situé dans le dossier `public` pour des raisons de sécurité, séparé des autres composants de l'application.

Configurez votre serveur web pour qu'il pointe directement vers le dossier `public/`. Il est recommandé d'utiliser un hôte virtuel pour une gestion optimale.

## Fonctionnalités Clés

- Limitation à 50 relations par utilisateur pour encourager des connexions de qualité.
- Limitation à 10 publications par jour pour éviter la surcharge d'informations.
- Design inspiré de réseaux sociaux comme Twitter et Reddit.
- Gestion intuitive et légère grâce à CodeIgniter 4.

## Requêtes Serveur

MyLittleClub nécessite les configurations suivantes :

- PHP version 7.4 ou supérieure (recommandé : PHP 8.1 ou plus récent).
- Extensions PHP nécessaires :  
  - `intl`  
  - `mbstring`  
  - `json` (activé par défaut)  
  - `mysqlnd` (si MySQL est utilisé)  
  - `libcurl` (si vous utilisez HTTP\CURLRequest)

⚠️ Attention : PHP 7.4 a atteint sa fin de vie en novembre 2022. PHP 8.0 a également atteint sa fin de vie en novembre 2023. Assurez-vous d'utiliser une version prise en charge, comme PHP 8.1 ou ultérieure.

## Contribution

Pour signaler des problèmes ou proposer des idées :

- Utilisez les issues GitHub de ce dépôt pour les bogues et suggestions.
- Discutez des nouvelles fonctionnalités via des demandes ou sur le forum associé.

## Ressources Utiles

- Documentation CodeIgniter : [CodeIgniter User Guide](https://codeigniter.com/user_guide/)
- Dépôt Principal : Suivez les mises à jour et les fonctionnalités sur le dépôt principal de CodeIgniter.

---

# CodeIgniter 4 Application Starter

## Qu'est-ce que CodeIgniter ?

CodeIgniter est un framework PHP full-stack, léger, rapide, flexible et sécurisé. Pour plus d'informations, consultez le [site officiel](https://codeigniter.com).

Ce dépôt contient un starter d'application installable via Composer, construit à partir du [dépôt de développement](https://github.com/codeigniter4/CodeIgniter4).

Pour plus d'informations sur la version 4, consultez [CodeIgniter 4](https://forum.codeigniter.com/forumdisplay.php?fid=28) sur les forums.

Vous pouvez lire le [guide de l'utilisateur](https://codeigniter.com/user_guide/) correspondant à la dernière version du framework.

## Installation et Mises à Jour

1. Exécutez `composer create-project codeigniter4/appstarter` puis `composer update` à chaque nouvelle version du framework.
2. Lors de la mise à jour, consultez les notes de version pour vérifier s'il y a des modifications à apporter à votre dossier `app`. Les fichiers concernés peuvent être copiés ou fusionnés depuis `vendor/codeigniter4/framework/app`.

## Configuration

Copiez le fichier `env` en `.env` et personnalisez-le pour votre application, notamment le `baseURL` et les paramètres de la base de données.

## Changement Important avec `index.php`

Le fichier `index.php` n'est plus situé à la racine du projet ! Il a été déplacé dans le dossier *public* pour améliorer la sécurité et séparer les composants.

Cela signifie que vous devez configurer votre serveur web pour qu'il pointe vers le dossier *public* du projet, et non vers la racine. Une meilleure pratique consiste à configurer un hôte virtuel pour pointer vers ce dossier. Il est déconseillé de pointer votre serveur web vers la racine du projet et d'attendre d'entrer dans *public/...*.

**Veuillez** lire le guide de l'utilisateur pour une meilleure compréhension de la structure de CodeIgniter 4 !

## Gestion du Dépôt

Nous utilisons les issues GitHub sur notre dépôt principal pour suivre les **BUGS** et les **PAQUETS DE TRAVAIL** approuvés pour le développement.  
Nous utilisons notre [forum](http://forum.codeigniter.com) pour fournir du support et discuter des **DEMANDES DE FONCTIONNALITÉS**.

Ce dépôt est une "distribution" construite par notre script de préparation des versions. Les problèmes liés à ce dépôt peuvent être soulevés sur notre forum ou comme des issues dans le dépôt principal.

## Exigences Serveur

PHP version 7.4 ou plus récente, avec les extensions suivantes installées :

- [intl](http://php.net/manual/en/intl.requirements.php)
- [mbstring](http://php.net/manual/en/mbstring.installation.php)

> [!AVERTISSEMENT]  
> La fin de vie pour PHP 7.4 a eu lieu le 28 novembre 2022.  
> La fin de vie pour PHP 8.0 a eu lieu le 26 novembre 2023.  
> Si vous utilisez encore PHP 7.4 ou 8.0, vous devez mettre à jour immédiatement.  
> La fin de vie pour PHP 8.1 est prévue pour le 25 novembre 2024.

De plus, assurez-vous que les extensions suivantes sont activées dans votre PHP :

- `json` (activé par défaut - ne le désactivez pas)
- [mysqlnd](http://php.net/manual/en/mysqlnd.install.php) si vous prévoyez d'utiliser MySQL
- [libcurl](http://php.net/manual/en/curl.requirements.php) si vous prévoyez d'utiliser la bibliothèque HTTP\CURLRequest
