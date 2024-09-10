### Analyse et modélisation prédictive pour un site de pari en ligne : Évaluation des performances des utilisateurs et prévision des comportements de paris en ligne.

# Projet d'analyse des données et de machine learning pour BetSmart

## Aperçu du projet

Ce projet se concentre sur l'analyse du comportement des utilisateurs de la plateforme BetSmart, un site de paris en ligne dédié au football. L'objectif de ce projet est de :

1. **Tester l'efficacité** d'une nouvelle fonctionnalité qui prédit les résultats des matchs pour les utilisateurs premium.
2. **Fournir des insights** basés sur l'analyse des données et suggérer des stratégies pour améliorer l'engagement des clients.
3. **Développer des modèles prédictifs** pour prévoir le comportement des clients, notamment la probabilité qu'un pari soit gagnant et qu'un client standard passe à un compte premium.

## Jeux de données

Trois jeux de données ont été utilisés pour cette analyse :

1. **bets.csv** : Contient des informations détaillées sur les paris effectués sur la plateforme.
2. **customers.csv** : Contient des informations sur les clients, notamment s'ils sont des utilisateurs premium et s'ils ont eu accès au nouveau service de prédiction.
3. **pricing.csv** : Contient les détails des tarifs d'abonnement pour les comptes standard et premium.

## Objectifs clés

1. **Test de la fonctionnalité** : Analyser si la nouvelle fonctionnalité, offerte aux utilisateurs premium entre le 14 juin 2018 et le 15 juillet 2018, a amélioré leur expérience de pari.
2. **Développement des KPIs** : Créer un tableau de bord pour suivre la performance de l'entreprise.
3. **Machine Learning** : Implémenter des modèles prédictifs pour anticiper des résultats tels que la victoire d'un pari ou la conversion d'un client standard en compte premium.

## Outils et techniques utilisés

- **Prétraitement des données** : pandas, NumPy
- **Visualisation des données** : Matplotlib, Seaborn
- **Machine Learning** : scikit-learn, RandomForestClassifier, LogisticRegression
- **Évaluation des modèles** : Précision, rappel, matrice de confusion

## Structure du projet

```
├── data
│   ├── bets.csv
│   ├── customers.csv
│   ├── pricing.csv
├── notebooks
│   ├── 01_data_analysis.ipynb
│   ├── 02_machine_learning_models.ipynb
├── README.md
```

## Résultats clés de l'analyse

1. **Analyse du comportement des clients** : Il n'y a pas eu d'amélioration significative du taux de réussite des paris pour les clients ayant eu accès au nouveau service, indiquant que ce dernier n'a pas eu un impact majeur sur leur comportement de pari.
2. **Tableau de bord KPI** : Les tendances des abonnements mensuels et les commissions des paris ont été suivies pour évaluer la performance de l'entreprise.
3. **Modèles de Machine Learning** :
   - **Prédiction du résultat des paris** : Un modèle Random Forest a été entraîné pour prédire si un pari sera gagnant ou perdant en fonction des caractéristiques disponibles.
   - **Conversion des clients** : Un modèle de régression logistique a été utilisé pour prédire si un client standard passera à un compte premium.

## Modèles de Machine Learning

### Modèle 1 : Prédiction des résultats des paris

Le modèle Random Forest a été entraîné en utilisant des caractéristiques telles que la valeur du pari, le statut premium et l'accès au service de test pour prédire la probabilité qu'un pari soit gagnant. Le modèle a atteint une précision raisonnable, mais pourrait être amélioré avec plus de fonctionnalités et un réglage des hyperparamètres.

### Modèle 2 : Conversion des clients standard en premium

Un modèle de régression logistique a été utilisé pour prédire la probabilité qu'un client passe d'un compte standard à un compte premium. Le modèle offre des insights précieux sur les facteurs qui influencent cette conversion.
