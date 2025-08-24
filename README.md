## Projet : Création d'un Classificateur pour Prédire l'Attrition des Clients de SyriaTel

### Aperçu du projet
Développer un modèle prédictif pour identifier les clients susceptibles de résilier leur 
abonnement (phénomène de churn), afin de permettre une intervention proactive et personnalisée.

#### Données utilisées
* Source : bigml_59.csv
* Nombre de clients : 3 333
* Nombre de caractéristiques : 21 variables (démographiques, comportementales, contrat)

#### Type de données
* Durée du compte
* Minutes d’appel (jour, soir, nuit)
* Type d’abonnement (international, messagerie vocale)
* Nombre d’appels au service client
  
#### Méthodologie
* Nettoyage et préparation des données
* Aucune valeur manquante détectée
* Encodage des variables catégorielles (ex: "international plan" → oui/non → 1/0)
* Standardisation des données numériques

#### Exploration des données (EDA)
* Taux d’attrition : 14,5% des clients ont résilié
* Variables les plus corrélées au churn :
* Abonnement international
* Nombre d’appels au service client
* Minutes et coût des appels de jour

#### Modélisation
Algorithmes testés :
* Random Forest
* Gradient Boosting
* Régression Logistique

#### Optimisation :
Réglage fin des hyperparamètres via validation croisée.

Résultats principaux Performance du meilleur modèle

* Précision : > 90%
* AUC (courbe ROC) : > 0,95 → excellente capacité à distinguer les clients à risque

#### Variables les plus importantes

1. Nombre d’appels au service client : plus il est élevé, plus le risque de résiliation est grand.
2. Abonnement international : les clients avec un forfait international ont un risque accru.
3. Minutes d’appel de jour : une utilisation élevée est corrélée à un risque plus faible.

##### Applications concrètes
##### Actions recommandées

* Cibler les clients à risque : offrir des promotions personnalisées, un support renforcé.
* Améliorer le service client : réduire le nombre d’appels nécessaires.
* Adaptateur les offres : revoir les forfaits internationaux pour les rendre plus attractifs.
  
#### Bénéfices attendus
* Réduction du taux d’attrition
* Augmentation de la fidélisation
* Optimisation des campagnes marketing

#### Perspectives
* Intégration en temps réel des prédictions dans l’outil de gestion client
* Ajout de données externes (ex: satisfaction client)
* Automatisation des actions de rétention

#### Conclusion
Ce modèle permet une détection précoce et fiable des clients à risque 
de résiliation, offrant ainsi des opportunités concrètes 
pour améliorer la rétention et la rentabilité.
