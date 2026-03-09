# Dataset: LOSC Match History (2005-2024)

Ce répertoire contient les données brutes utilisées pour la simulation via échantillonnage préférentiel.

Ce jeu de données comprend **n = 746 observations** correspondant aux matchs de championnat du LOSC Lille sur 20 saisons (2005-2024). Les données ont été extraites du site officiel de la [Ligue 1](https://ligue1.fr).

### Structure des données
La variable principale du fichier est l'écart de buts par match ($X_i$), calculée comme suit :
$$X_i = \text{Buts marqués} - \text{Buts concédés}$$

* **$X_i > 0$** : Victoire du LOSC ;
* **$X_i = 0$** : Match nul ;
* **$X_i < 0$** : Défaite du LOSC.

### Statistiques descriptives
* **Moyenne ($\mu$)** : 0,42
* **Écart-type ($\sigma$)** : 1,63
* **Minimum** : -6 (Plus large défaite)
* **Maximum** : 8 (Plus large victoire)

---

## English Version

This directory contains the historical data used for the Importance Sampling simulation.

### Dataset Overview
The dataset consists of **n = 746 observations** from LOSC Lille league matches over 20 seasons (2005-2024). Data was sourced from the official [Ligue 1](https://ligue1.fr) website.

### Data Structure
The primary variable is the goal difference per match ($X_i$), calculated as:
$$X_i = \text{Goals Scored} - \text{Goals Conceded}$$

* **$X_i > 0$**: LOSC Victory
* **$X_i = 0$**: Draw
* **$X_i < 0$**: LOSC Defeat

### Key Metrics
* **Mean ($\mu$)**: 0.42
* **Standard Deviation ($\sigma$)**: 1.63
* **Minimum**: -6 (Largest defeat)
* **Maximum**: 8 (Largest victory)