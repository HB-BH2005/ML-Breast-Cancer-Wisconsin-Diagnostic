# Analyse et Classification du Cancer du Sein

## Introduction
Ce notebook est dédié à l'analyse et à la classification du cancer du sein en utilisant le jeu de données *Breast Cancer Wisconsin (Diagnostic)*. L'objectif principal est de développer et de comparer divers modèles de machine learning pour prédire la malignité d'une tumeur (bénigne ou maligne) à partir de caractéristiques morphologiques des cellules. Un accent particulier est mis sur la précision de la détection des cas malins (minimisation des faux négatifs).

## Problématique
Le cancer du sein est un problème de santé majeur. Un diagnostic précoce et précis est essentiel pour un traitement efficace. Notre but est d'identifier le modèle de classification le plus performant pour cette tâche, en privilégiant la **précision pour la classe Maligne (classe 0)**, afin de garantir qu'un maximum de cas de cancer sont correctement identifiés, même au prix d'un léger augmentation des faux positifs.

## Jeu de Données
Le jeu de données est fourni par l'UCI Machine Learning Repository (ID 17). Il contient des caractéristiques numériques calculées à partir d'une image numérisée d'une masse mammaire. Chaque observation représente une tumeur, caractérisée par 30 attributs, et une variable cible (`Diagnosis` ou `target`) indiquant si la tumeur est Maligne (M, encodée en 0) ou Bénigne (B, encodée en 1).

Les caractéristiques sont divisées en trois catégories pour chaque mesure (e.g., `radius`, `texture`, `perimeter`, `area`, `smoothness`, `compactness`, `concavity`, `concave_points`, `symmetry`, `fractal_dimension`):
- `_mean`: La moyenne de la caractéristique.
- `_se`: L'erreur standard de la caractéristique.
- `_worst`: La 
