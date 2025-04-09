# Analyse de l'Égalité Hommes / Femmes - Workflow KNIME

## 🧠 Objectif du projet

Ce projet a pour but d'étudier les inégalités potentielles entre les femmes et les hommes dans le monde professionnel à partir de données RH. Il s’inscrit dans le cadre d’un projet d’étude portant sur l’égalité de traitement à différents niveaux (rémunération, embauche, qualification, etc.).

L’ensemble du processus est implémenté via **KNIME**, une plateforme d’analyse de données open source, permettant de visualiser les étapes de traitement et d’analyse de manière transparente.

---

## 📂 Structure du projet

Le projet est divisé en plusieurs parties visibles dans le workflow principal :

### 1. Accès aux données
- Import des données RH depuis Google Drive et Excel.
- Données concernées :
  - Informations professionnelles
  - Rémunération
  - Salaires
  - Tâches

### 2. Nettoyage et transformation
- Traitement des valeurs manquantes
- Normalisation et transformation des données
- Calculs de colonnes intermédiaires :
  - Dates d’entrée/sortie
  - Durée de présence
  - Temps complet/partiel
- Regroupement par sexe pour analyse comparative

### 3. Analyses statistiques
- **Test de normalité** (Shapiro-Wilk)
- **Test de Kruskal-Wallis** pour analyser les différences significatives entre groupes (qualitatif vs quantitatif)
- **Test du Chi-deux** via table de contingence (relation entre variables catégorielles)

### 4. Analyses spécifiques
- **Rémunération** : Comparaison des salaires moyens et écarts par sexe
- **Embauche** : Répartition des embauches par sexe et type de contrat
- **Qualification** : Répartition des niveaux de qualification par service
- **Accès à la formation** : Égalité d’accès à la formation
- **Classification des métiers** : Analyse des postes occupés
- **Entretien annuel** : Taux d’entretien réalisé par sexe

---

## 🔍 Visualisation

Le projet comprend un **workflow global** sous forme de schéma KNIME (`Workflow_Egalité_H:F.png`), ainsi que des **captures zoomées** des différentes sections pour faciliter la lecture et la compréhension (`image.png`).

---

## 🛠️ Technologies utilisées

- **KNIME Analytics Platform**
- **Tests statistiques** intégrés (Python / R intégrés à KNIME si besoin)
- **Excel / Google Sheets** pour les données sources

---

## 📈 Résultats attendus

- Identification d’inégalités de traitement potentielles
- Visualisation claire des points de friction dans le parcours professionnel
- Proposition de pistes d’amélioration pour plus d’équité

---
## 🔄 Aperçu du Workflow KNIME

Voici une vue d’ensemble du workflow utilisé dans ce projet :

![Aperçu du Workflow KNIME](Workflow_Egalité_H:F.png)

## 📎 Fichiers
- Workflow : A ouvrir avec KNIME déjà installé sur PC
- `Workflow_Egalité_H/F.png` : Vue d’ensemble du workflow KNIME
- `images.png` : Zoom sur les différentes sections du projet
- `README.md` : Fichier de documentation du projet
