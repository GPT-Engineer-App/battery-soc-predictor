# battery-soc-predictor

développe un script Matlab d'un modèle d’estimation ou prédiction de l’état de charge (SoC) des batteries de voiture électrique en utilisant le modèle de Support Vector Machine (SVM) avec différents types de noyaux, et de déterminer celui qui offre les meilleures performances.     Ces données contenant :
•	Données environnementales (température, altitude, etc.)
•	Données du véhicule (vitesse, accélérateur, etc.)
•	Données relatives à la batterie (tension, courant, température, SoC)
•	Données du circuit de chauffage (température intérieure, puissance de chauffage, etc.)
seront utilisées pour entraîner et tester le modèle SVM afin d'estimer ou de prédire l'état de charge.   1.   Les données sont collectées comme suite à partir de véhicules électriques les mesures de tension, de courant, de température, etc.
Les données de mesure sont classées en deux catégories. La catégorie A(TripA05), enregistrée durant l'été, est incomplète en raison d'un dysfonctionnement du système de mesure, tandis que la catégorie B(TripB05), enregistrée pendant l'hiver, est complète et cohérente.    2. Dans le Prétraitement des données tu nettoieras les données ce qui est nécessaire afin d'identifier et de traiter les valeurs aberrantes, manquantes ou des potentielles erreurs des données, après le nettoyage il y aura la normalisation mettre à l'échelle les caractéristiques pour assurer une convergence plus rapide et une meilleure performance des modèles.    3. Tu définiras les caractéristiques (feature) et de la cible et ces  caractéristiques incluront les mesures de tension, de courant, de température, etc., ainsi que des caractéristiques dérivées telles que la puissance et l'état de charge précédent. Tout en sachant que la cible sera l'état de charge réel de la batterie à un instant donné.      4. Le choix du modèle sera un modèle SVM qui sera utilisé pour prédire l'état de charge des batteries de voiture électrique en utilisant différents types de noyaux. Ces types de noyaux à tester incluront : linéaire, polynomial et gaussien (RBF). Après il va falloir déterminer les hyper-paramètres des modèles SVM qui seront optimisés par validation croisée pour chaque type de noyau.	  5. Dans l'entraînement et évaluation des modèles tu dois diviser les données en ensembles d'entraînement et de test juste après tu dois entraîner le modèle SVM avec chaque type de noyau en utilisant l'ensemble d'entraînement en suite tu dois évaluer les performances de chaque modèle en utilisant l'ensemble de test, en utilisant des métriques telles que le coefficient de corrélation (R), l'erreur absolue moyenne (MAE), l'erreur quadratique moyenne (RMSE), etc.  6. Dans analyse des résultats tu dois comparer les performances des différents types de noyaux en terme de précision de la prédiction de l'état de charge et identifier le noyau qui offre les meilleurs performances et le sélectionner comme modèle final mais en affichant aussi les autres modèles.  7. tu présente les résultats sous forme de graphiques, de tableaux et de métriques de performance pour chaque type de noyau puis fourni une analyse des avantages et des inconvénients de chaque noyau dans le contexte de la prédiction de l'état de charge des batteries de voiture électrique. tu dois ploter les résultats d'entraînement et de test sur des figure différentes tous les résulter si possible


## Collaborate with GPT Engineer

This is a [gptengineer.app](https://gptengineer.app)-synced repository 🌟🤖

Changes made via gptengineer.app will be committed to this repo.

If you clone this repo and push changes, you will have them reflected in the GPT Engineer UI.

## Tech stack

This project is built with React and Chakra UI.

- Vite
- React
- Chakra UI

## Setup

```sh
git clone https://github.com/GPT-Engineer-App/battery-soc-predictor.git
cd battery-soc-predictor
npm i
```

```sh
npm run dev
```

This will run a dev server with auto reloading and an instant preview.

## Requirements

- Node.js & npm - [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating)
