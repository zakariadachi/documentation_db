Fondamentaux des bases de données
1. Ce qu’il faut apprendre
1.1 Qu’est-ce qu’une base de données et pourquoi en a-t-on besoin ?

Une base de données est un espace numérique qui permet de stocker des informations de manière organisée afin de pouvoir les utiliser facilement par la suite.
Elle remplace les fichiers classiques (papier, Excel, dossiers) lorsque les données deviennent nombreuses.

Pourquoi utiliser une base de données :

Pour organiser les données correctement

Pour accéder rapidement aux informations

Pour éviter les erreurs et les doublons

Pour sécuriser les données

Pour permettre à plusieurs utilisateurs d’accéder aux mêmes données

Exemple :
Un site web utilise une base de données pour stocker les utilisateurs, les articles et les commentaires.

1.2 Types de bases de données (Relationnelles vs NoSQL)
A. Bases de données relationnelles

Les bases de données relationnelles stockent les données dans des tables composées de lignes et de colonnes.
Les tables peuvent être liées entre elles grâce aux clés.

Caractéristiques :

Structure claire et fixe

Utilisation du langage SQL

Très utilisées dans les applications classiques

Exemples :

MySQL

PostgreSQL

Oracle

SQL Server

B. Bases de données NoSQL

Les bases de données NoSQL sont plus flexibles et ne suivent pas toujours le modèle des tables.

Caractéristiques :

Données non structurées ou semi-structurées

Très rapides et évolutives

Utilisées pour les grandes applications

Exemples :

MongoDB

Redis

Cassandra

1.3 Comprendre un DBMS (Database Management System)

Un DBMS est un logiciel qui permet de créer, gérer et contrôler une base de données.
Il agit comme un intermédiaire entre l’utilisateur et les données.

Rôles principaux du DBMS :

Créer des bases et des tables

Ajouter, modifier et supprimer des données

Gérer les utilisateurs et les permissions

Assurer la sécurité et les sauvegardes

Exemples de DBMS :

MySQL

PostgreSQL

Oracle DB

MongoDB

1.4 Applications réelles des bases de données

Les bases de données sont utilisées dans presque tous les domaines :

Sites web et applications

Banques et systèmes de paiement

Écoles et universités

Hôpitaux

E-commerce

Réseaux sociaux

Exemple concret :
Un site de vente en ligne utilise une base de données pour gérer les produits, les commandes et les clients.

1.5 Aperçu de l’architecture d’une base de données

L’architecture décrit comment les différents éléments communiquent entre eux.

Architecture classique client–serveur :

Client : navigateur ou application

Serveur : application backend

Base de données : stockage des données

Fonctionnement :
Le client envoie une demande → le serveur traite → la base de données répond → le résultat revient au client.

2. Ce qu’il faut documenter
2.1 Différences clés entre les types de bases de données

Relationnelles : structure fixe, SQL

NoSQL : structure flexible, grande performance

2.2 DBMS populaires et leurs cas d’utilisation

MySQL : sites web et projets moyens

PostgreSQL : applications complexes

MongoDB : données flexibles et Big Data

2.3 Diagramme des composants d’une base de données

Un schéma montrant :

Utilisateur

Application

DBMS

Base de données

2.4 Avantages des bases de données par rapport aux fichiers

Meilleure organisation

Sécurité des données

Accès rapide

Travail collaboratif

Sauvegarde automatique

3. Ce qu’il faut maîtriser
3.1 Terminologie des bases de données

Comprendre les mots clés :

Base de données

Table

Enregistrement

Champ

Clé primaire

Clé étrangère

DBMS

3.2 Choisir le bon type de base selon le besoin

Données structurées → base relationnelle

Données flexibles → NoSQL

3.3 Comprendre l’architecture client–serveur

Savoir expliquer comment une application communique avec une base de données via un serveur.