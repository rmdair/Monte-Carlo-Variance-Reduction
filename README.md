<h1 align="center">Réduction de la variance en simulation de Monte-Carlo</h1>

---

<p align="center">
  <img src="https://img.shields.io/badge/R_Language-276DC3?style=flat-square&logo=R" alt="R">
  <img src="https://img.shields.io/badge/License-MIT-darkgreen?style=flat-square" alt="License">
</p>

<p align="center">
  <img src="assets/banner.webp" alt="Banner" width="60%">
</p>

Les simulations de Monte-Carlo sont des outils puissants pour estimer des quantités probabilistes complexes, mais elles souffrent souvent d'une variance élevée qui peut limiter leur efficacité, notamment dans l'étude des **événements rares**. Ce projet explore trois méthodes majeures de **réduction de la variance** pour améliorer la précision et réduire le coût computationnel :

1. **Échantillonnage préférentiel (Importance Sampling)** : Modifie la distribution d'échantillonnage pour mieux capter les événements rares ;
2. **Variables de contrôle** : Exploite la corrélation entre variables aléatoires pour réduire la variance de l'estimateur ;
3. **Stratification** : Segmente l’espace d’échantillonnage en groupes homogènes pour affiner les estimations.

L’approche théorique est complétée par une **application concrète au domaine du sport**, en évaluant la probabilité d’un score exceptionnel dans un match de football du LOSC Lille.

---

## Ressources

Le rapport couvre les aspects suivants :
- Fondements théoriques des simulations de Monte Carlo.
- Présentation détaillée des méthodes de réduction de la variance.
- Quelques démonstrations mathématiques des propriétés fondamentales.
- Comparaison des performances des méthodes sur des cas concrets.
- Application aux données du LOSC pour estimer la probabilité d’une victoire par au moins 8 buts d’écart.

| Document | Langue | Lien |
| :--- | :--- | :--- |
| Rapport Technique | Français | [Consulter PDF](./docs/Reduction-Variance-Monte-Carlo.pdf) |
| Technical Report | English | [View PDF](./docs/Monte-Carlo-Variance-Reduction.pdf) |


## Code et données  
Le projet inclut plusieurs implémentations en **R** (accessibles via [ce lien](src/)) :
- Estimation par variables de contrôle.
- Estimation par stratification.
- Analyse appliquée aux performances du LOSC via l'échantillonnage préférentiel.
  
Les variances associées à ces méthodes sont comparées avec l'approche de Monte-Carlo classique.

**Données utilisées :**  
Les données des matchs du LOSC (2005-2024), incluant le calcul des différences de buts, sont accessibles via le lien suivant :
[Consulter les données CSV](data/LOSC.csv)

## Installation et utilisation

Pour explorer le projet en local :

```bash
# Cloner le dépôt
git clone https://github.com/rmdair/Monte-Carlo-Variance-Reduction.git

# Accéder au dossier du projet
cd Monte-Carlo-Variance-Reduction
```

## Références  
- Rasmussen & Glynn, *Stochastic Simulation: Algorithms and Analysis*, Springer, 2009.  
- Christian P. Robert & George Casella, *Monte Carlo Statistical Methods*, Springer, 2004.  
- Rubinstein & Kroese, *Simulation and the Monte Carlo Method*, Wiley, 2016.  
- Pour la Science, n°385, *Hasard et incertitude, les défis qu’ils posent*, novembre 2009.  

