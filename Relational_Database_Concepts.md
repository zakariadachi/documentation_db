Phase 2 : Concepts des bases de données relationnelles
1. Ce qu’il faut apprendre
1.1 Tables, lignes et colonnes

Dans une base de données relationnelle, les informations sont organisées sous forme de tables.

Une table représente un sujet précis (exemple : utilisateurs, produits).

Une ligne (ou enregistrement) représente une seule information complète.

Une colonne (ou champ) représente un type de donnée précis.

Exemple :
Table users

Colonnes : id, nom, email

Chaque ligne : un utilisateur

1.2 Clés primaires et clés étrangères
Clé primaire (Primary Key)

La clé primaire est un champ qui permet d’identifier chaque ligne de manière unique dans une table.

Caractéristiques :

Unique

Non vide

Une seule par table

Exemple :
user_id dans la table users.

Clé étrangère (Foreign Key)

La clé étrangère est un champ qui permet de lier deux tables entre elles.

Exemple :
Dans la table articles, le champ user_id fait référence à la table users.

1.3 Relations entre les tables

Les relations définissent comment les tables sont connectées.

A. Relation Un-à-Un (One-to-One)

Une ligne d’une table correspond à une seule ligne dans une autre table.

Exemple :
Un utilisateur → un profil.

B. Relation Un-à-Plusieurs (One-to-Many)

Une ligne d’une table peut être liée à plusieurs lignes d’une autre table.

Exemple :
Un utilisateur → plusieurs articles.

C. Relation Plusieurs-à-Plusieurs (Many-to-Many)

Plusieurs lignes d’une table sont liées à plusieurs lignes d’une autre table.
On utilise une table intermédiaire.

Exemple :
Étudiants ↔ Cours.

1.4 Types de données et contraintes
Types de données

Ils définissent le type d’information stockée dans une colonne.

Exemples courants :

INT : nombres entiers

VARCHAR : texte

DATE : dates

FLOAT : nombres décimaux

BOOLEAN : vrai ou faux

Contraintes

Les contraintes assurent la validité des données.

Exemples :

NOT NULL : champ obligatoire

UNIQUE : valeur unique

PRIMARY KEY : identifiant unique

FOREIGN KEY : relation entre tables

1.5 Diagramme Entité-Relation (ERD)

Un ERD (Entity-Relationship Diagram) est un schéma visuel qui montre :

Les tables (entités)

Les colonnes

Les clés

Les relations entre les tables

Il permet de concevoir la base de données avant de la créer.

2. Ce qu’il faut documenter
2.1 ERD pour un cas réel

Créer un ERD pour un exemple comme :

Blog

Boutique en ligne

Gestion d’étudiants

2.2 Types de relations avec exemples

Documenter :

One-to-One

One-to-Many

Many-to-Many
avec des schémas simples.

2.3 Guide des types de données

Un tableau qui explique :

Le type

Son usage

Des exemples

2.4 Types de contraintes et leurs rôles

Expliquer pourquoi chaque contrainte est utilisée et ce qu’elle empêche.

3. Ce qu’il faut maîtriser
3.1 Concevoir un schéma simple

Être capable de :

Identifier les tables nécessaires

Définir les colonnes

Choisir les clés primaires

3.2 Créer et lire un ERD

Savoir :

Dessiner un ERD

Comprendre un ERD existant

3.3 Implémenter des relations correctes

Savoir :

Quand utiliser une clé étrangère

Comment créer une table intermédiaire

Respecter l’intégrité des données