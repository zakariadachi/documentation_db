Phase 4 : Requêtes SQL avancées
1. Ce qu’il faut apprendre
1.1 Les opérations JOIN

Les JOIN permettent de combiner des données provenant de plusieurs tables liées entre elles.

INNER JOIN

Retourne uniquement les lignes qui ont une correspondance dans les deux tables.

Exemple :
Afficher les articles avec le nom de leur auteur.

SELECT users.name, articles.title
FROM users
INNER JOIN articles ON users.id = articles.user_id;

LEFT JOIN

Retourne toutes les lignes de la table de gauche, même si aucune correspondance n’existe dans la table de droite.

Exemple :
Afficher tous les utilisateurs, même ceux qui n’ont pas d’articles.

SELECT users.name, articles.title
FROM users
LEFT JOIN articles ON users.id = articles.user_id;

RIGHT JOIN

Retourne toutes les lignes de la table de droite.

Exemple :

SELECT users.name, articles.title
FROM users
RIGHT JOIN articles ON users.id = articles.user_id;

FULL JOIN

Retourne toutes les lignes des deux tables, avec ou sans correspondance.
(Utilisé surtout dans PostgreSQL et Oracle.)

1.2 Fonctions d’agrégation

Les fonctions d’agrégation permettent de faire des calculs sur plusieurs lignes.

COUNT() : compter le nombre de lignes

SUM() : calculer un total

AVG() : calculer une moyenne

MAX() : valeur maximale

MIN() : valeur minimale

Exemple :

SELECT COUNT(*) FROM users;

1.3 GROUP BY et HAVING
GROUP BY

Permet de regrouper les données selon une colonne.

Exemple :
Nombre d’articles par utilisateur.

SELECT user_id, COUNT(*) 
FROM articles
GROUP BY user_id;

HAVING

Permet de filtrer les groupes, contrairement à WHERE qui filtre les lignes.

Exemple :

SELECT user_id, COUNT(*) 
FROM articles
GROUP BY user_id
HAVING COUNT(*) > 2;

1.4 Sous-requêtes (Subqueries)

Une sous-requête est une requête SQL à l’intérieur d’une autre requête.

Exemple :
Afficher les utilisateurs qui ont écrit au moins un article.

SELECT name 
FROM users
WHERE id IN (
  SELECT user_id FROM articles
);

1.5 Opérations sur les ensembles

Les opérations sur les ensembles permettent de combiner plusieurs résultats.

UNION : combine les résultats sans doublons

INTERSECT : retourne les valeurs communes

EXCEPT : retourne les valeurs différentes

Exemple :

SELECT email FROM clients
UNION
SELECT email FROM subscribers;

2. Ce qu’il faut documenter
2.1 Comparaison des types de JOIN

Créer un tableau comparatif montrant :

Type de JOIN

Résultat

Cas d’utilisation

Exemple SQL

2.2 Cas d’utilisation des fonctions d’agrégation

Expliquer quand utiliser :

COUNT pour les statistiques

SUM pour les totaux

AVG pour les moyennes

2.3 Modèles de sous-requêtes et bonnes pratiques

Documenter :

Sous-requêtes avec IN

Sous-requêtes avec EXISTS

Éviter les sous-requêtes inutiles

2.4 Conseils d’optimisation des requêtes complexes

Utiliser des index

Éviter SELECT *

Limiter les résultats

Tester les performances

3. Ce qu’il faut maîtriser
3.1 Écrire des requêtes multi-tables

Être capable de :

Relier plusieurs tables

Choisir le bon type de JOIN

Lire des requêtes complexes

3.2 Créer des rapports avec agrégation

Savoir :

Compter

Regrouper

Analyser des données

3.3 Résoudre des problèmes métiers complexes

Utiliser SQL pour :

Analyser des ventes

Suivre des utilisateurs

Générer des statistiques réelles