Phase 3 : Bases du langage SQL
1. Ce qu’il faut apprendre
1.1 Syntaxe et structure du SQL

SQL (Structured Query Language) est le langage utilisé pour communiquer avec une base de données relationnelle.
Il permet de créer des tables, d’ajouter des données et de les consulter.

Structure générale d’une requête SQL :

Les mots-clés sont en anglais (SELECT, FROM, WHERE…)

Les commandes sont claires et lisibles

Chaque requête se termine par un point-virgule ;

Exemple simple :

SELECT * FROM users;


Cette requête affiche tous les utilisateurs.

1.2 Data Definition Language (DDL)

Le DDL regroupe les commandes qui servent à créer et modifier la structure de la base de données.

Commandes principales :

CREATE : créer une base ou une table

ALTER : modifier une table existante

DROP : supprimer une table ou une base

Exemple :

CREATE TABLE users (
  id INT PRIMARY KEY,
  name VARCHAR(50)
);

1.3 Data Manipulation Language (DML)

Le DML permet de gérer les données à l’intérieur des tables.

Commandes principales :

INSERT : ajouter des données

UPDATE : modifier des données

DELETE : supprimer des données

Exemple :

INSERT INTO users (id, name) VALUES (1, 'Ali');

1.4 Requêtes SELECT de base

La commande SELECT est utilisée pour lire les données.

Exemples :

SELECT name FROM users;
SELECT * FROM users;


* signifie toutes les colonnes

On peut choisir une ou plusieurs colonnes

1.5 Filtrage et tri des données
Filtrage avec WHERE

La clause WHERE permet de filtrer les résultats.

Exemple :

SELECT * FROM users WHERE id = 1;

Tri avec ORDER BY

La clause ORDER BY permet de trier les résultats.

Exemple :

SELECT * FROM users ORDER BY name ASC;

Limitation avec LIMIT

LIMIT permet de limiter le nombre de résultats.

Exemple :

SELECT * FROM users LIMIT 5;

2. Ce qu’il faut documenter
2.1 Référence des commandes DDL

Documenter avec explications :

CREATE

ALTER

DROP

2.2 Référence des commandes DML

Documenter :

INSERT

UPDATE

DELETE
avec exemples pratiques.

2.3 Fiche des conditions WHERE

Inclure :

=, !=

>, <

LIKE

IN

BETWEEN

AND, OR

2.4 Exemples ORDER BY et LIMIT

Montrer comment trier :

Par ordre croissant (ASC)

Par ordre décroissant (DESC)

Limiter les résultats

3. Ce qu’il faut maîtriser
3.1 Créer et modifier les structures

Être capable de :

Créer une base

Créer une table

Modifier une table existante

3.2 Gérer les données

Savoir :

Insérer des données

Mettre à jour des informations

Supprimer des données en sécurité

3.3 Écrire des requêtes SELECT avec conditions

Maîtriser :

SELECT avec WHERE

SELECT avec ORDER BY

SELECT avec LIMIT