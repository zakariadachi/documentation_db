Phase 5 : Conception et normalisation des bases de données

1. Ce qu’il faut apprendre
   1.1 Le processus de conception d’une base de données

La conception d’une base de données consiste à organiser les données de manière logique avant de les créer techniquement.

Étapes principales :

Analyse des besoins (quelles données stocker ?)

Identification des entités (tables)

Définition des relations

Choix des clés primaires et étrangères

Normalisation

Implémentation dans le DBMS

Objectif :
Créer une base claire, évolutive et facile à maintenir.

1.2 Les formes normales (Normal Forms)

La normalisation permet de réduire les doublons et d’améliorer la cohérence des données.

Première forme normale (1NF)

Les colonnes contiennent des valeurs simples

Pas de listes ou de valeurs multiples dans une même colonne

Exemple incorrect :
phones = "0611, 0622"

Deuxième forme normale (2NF)

La table est en 1NF

Toutes les colonnes dépendent entièrement de la clé primaire

Troisième forme normale (3NF)

La table est en 2NF

Pas de dépendance entre colonnes non clés

BCNF (Boyce-Codd Normal Form)

Version plus stricte de la 3NF

Utilisée dans les bases complexes

1.3 La dénormalisation

La dénormalisation consiste à ajouter volontairement de la redondance pour améliorer les performances.

Quand l’utiliser :

Bases très sollicitées

Rapports complexes

Applications à grande échelle

Attention :
Elle doit être utilisée avec précaution.

1.4 Indexation et performance

Un index permet d’accélérer la recherche des données, comme un index dans un livre.

Types courants d’index :

Index simple

Index unique

Index composite

Avantages :

Requêtes plus rapides

Meilleures performances

Inconvénient :

Légère perte de performance lors des insertions

1.5 Intégrité et validation des données

L’intégrité des données garantit que les informations sont correctes et cohérentes.

Moyens utilisés :

Clés primaires

Clés étrangères

Contraintes (NOT NULL, UNIQUE, CHECK)

Validation côté application

2. Ce qu’il faut documenter
   2.1 Processus de normalisation (cas pratique)

Expliquer comment passer :

D’une table non normalisée

À une table en 3NF

2.2 Types d’index et cas d’utilisation

Documenter :

Quand utiliser un index

Sur quelles colonnes

Les impacts sur les performances

2.3 Exemples de règles de validation

Inclure :

Email valide

Champ obligatoire

Valeurs autorisées

2.4 Checklist d’optimisation des performances

Index bien placés

Requêtes optimisées

Données normalisées

Pas de redondance inutile

3. Ce qu’il faut maîtriser
   3.1 Concevoir des schémas normalisés

Être capable de :

Créer des tables claires

Appliquer la normalisation

Réduire les doublons

3.2 Créer des index efficaces

Savoir :

Choisir les bonnes colonnes

Éviter trop d’index

Tester les performances

3.3 Garantir l’intégrité des données

Maîtriser :

Les contraintes SQL

Les relations entre tables

La validation des données
