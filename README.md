# Projet de Prédiction des Incendies

## Objectif du Projet

Ce projet vise à prédire les occurrences d'incendies dans deux pays spécifiques, le Portugal et la Grèce. En utilisant des données historiques d'incendies, des informations météorologiques et des données de végétation, nous développons des modèles de machine learning pour effectuer une tâche de classification binaire (fire/not fire).

## Sources de Données

Les données utilisées dans ce projet proviennent de plusieurs sources :

- **Données MODIS** : Données historiques des incendies provenant de satellites, couvrant le Portugal et la Grèce pour l'année 2023.
- **API Météorologique** : Caractéristiques météorologiques extraites avant les incendies pour améliorer les prédictions.

## Structure des Notebooks

Le projet est organisé en quatre notebooks principaux, chacun gérant une étape spécifique du processus :

1. **Fire_Data** :
   - Chargement et traitement des données MODIS pour le Portugal et la Grèce.
   - Génération de données correspondantes à des événements 'not fire' pour introduire une tâche de classification binaire.

2. **Weather_Data** :
   - Extraction des caractéristiques météorologiques via une API, ciblant les conditions avant les incidents d'incendie pour enrichir le modèle de prédiction.

3. **Vegetation_Data** :
   - Collection et manipulation des données de végétation à partir de fichiers HDF, utilisant des techniques de géolocalisation pour préciser les zones d'étude.

4. **Modelisation_Evaluation** :
   - Fusion des données collectées, prétraitement, réduction de dimensionnalité, et construction de différents modèles de machine learning.
   - Évaluation et comparaison des modèles en utilisant diverses métriques de performance.

## Datasets

Le projet utilise un total de huit datasets distincts, qui incluent des données d'incendie, météorologiques, et de végétation pour les deux pays étudiés. Ces datasets sont préparés et nettoyés dans les différents notebooks avant d'être utilisés pour la modélisation.

## Comment Utiliser

Pour exécuter ce projet, commencez par le notebook `Fire_Data` pour la préparation initiale des données, suivi de `Weather_Data` et `Vegetation_Data` pour la collecte supplémentaire de données. Enfin, utilisez le notebook `Modelisation_Evaluation` pour la construction et l'évaluation des modèles prédictifs.

Chaque notebook est auto-contenu et peut être exécuté dans un environnement Jupyter avec les bibliothèques Python nécessaires installées, notamment scikit-learn, TensorFlow/Keras, Pandas, NumPy, et Seaborn/Matplotlib pour la visualisation.


