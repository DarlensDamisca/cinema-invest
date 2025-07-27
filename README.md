# cinema-invest
Films à produire pour maximiser les chances de succès commercial.

# 🎬 Analyse de Marché Cinématographique
## Recommandations Stratégiques pour un Nouveau Studio de Films

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 📋 Aperçu du Projet

Ce projet analyse les facteurs de succès dans l'industrie cinématographique pour guider les décisions de production d'un nouveau studio. En combinant les données IMDB et Box Office Mojo (2010-2018), nous identifions les genres, durées et niveaux de qualité qui maximisent la rentabilité.

### 🎯 Questions Business Clés

1. **Genres Rentables :** Quels genres de films génèrent le plus de revenus ?
2. **Durée Optimale :** Quelle durée maximise le succès commercial ?
3. **Impact Qualité :** Comment les notes influencent-elles la performance financière ?

---

## 🔍 Compréhension Business

### Contexte
Notre entreprise souhaite créer un nouveau studio de cinéma mais manque d'expertise dans l'industrie. Cette analyse fournit des recommandations basées sur des données pour minimiser les risques et maximiser les chances de succès commercial.

### Questions des Parties Prenantes
- **Directeur Studio :** "Quels types de films dois-je produire en priorité ?"
- **Investisseurs :** "Quel est le ROI attendu de chaque catégorie de film ?"
- **Équipe Créative :** "Comment équilibrer qualité artistique et succès commercial ?"

---

## 📊 Compréhension et Analyse des Données

### Sources des Données
- **IMDB Database** : 146,144 films avec notes, genres, durées
- **Box Office Mojo** : 3,387 films avec revenus domestiques/internationaux
- **Période** : 2010-2018 (données les plus fiables et récentes)

### Description des Données

#### Données IMDB
- `movie_id` : Identifiant unique du film
- `primary_title` : Titre principal du film  
- `start_year` : Année de sortie
- `genres` : Genres du film (format: "Genre1,Genre2,Genre3")
- `runtime_minutes` : Durée en minutes
- `averagerating` : Note moyenne (1-10)
- `numvotes` : Nombre de votes

#### Données Box Office  
- `title` : Titre du film
- `studio` : Studio de production
- `domestic_gross` : Revenus domestiques US ($)
- `foreign_gross` : Revenus internationaux ($)
- `year` : Année de sortie

### Préparation des Données
1. **Nettoyage** : Correction des formats de revenus, standardisation des titres
2. **Jointure** : Matching IMDB + Box Office sur titre et année
3. **Filtrage** : Films 2010-2018, revenus >$100K, durées réalistes (60-200 min)
4. **Enrichissement** : Calcul revenus totaux, catégorisation genres/durées/notes

---

## 📈 Visualisations Clés

### 1. Rentabilité par Genre
![Visualisation 1](images/visualisation_1_genres.png)

**Insights :**
- Les genres [X, Y, Z] dominent avec $XXM+ de revenus moyens
- Écart de XX% entre le genre le plus et le moins rentable
- Corrélation entre volume de production et rentabilité

### 2. Durée Optimale vs Performance  
![Visualisation 2](images/visualisation_2_duree.png)

**Insights :**
- Sweet spot identifié : XX-XX minutes
- Les films trop courts/longs sous-performent de XX%
- Durée optimale varie selon le genre

### 3. Impact des Notes sur le Succès
![Visualisation 3](images/visualisation_3_notes.png)

**Insights :**
- Corrélation qualité-revenus : X.XX
- Seuil critique : X.X/10 pour rentabilité optimale
- XX% des top revenus sont aussi bien notés

---

## 🎯 Conclusions

### Résumé des Découvertes

#### 🥇 Genre Prioritaire : [GENRE OPTIMAL]
- **Revenus moyens :** $XXM (+XX% vs moyenne)
- **Justification :** Performance consistante, marché établi
- **Recommandation :** 60% du budget de production

#### ⏱️ Durée Optimale : XX-XX minutes
- **Avantage :** +XX% revenus vs autres durées
- **Raisonnement :** Équilibre audience/exploitation cinéma
- **Application :** Standard pour films commerciaux

#### ⭐ Stratégie Qualité : Viser X.X+/10 IMDB
- **Impact :** +XX% revenus si seuil atteint
- **Équilibre :** Qualité ET éléments commerciaux
- **KPI :** Minimum X.X/10 pour validation projet

### 🎬 Recommandations Business

1. **Portfolio Diversifié :** 60% genre optimal, 30% genre secondaire, 10% innovation
2. **Métriques Cibles :** >$XXM revenus, >X.X/10 note, <24 mois ROI
3. **Gestion Risques :** Partenariats studios, veille marché, buffer budgétaire

### 💰 Impact Financier Estimé
- **Gain par film :** +$XXM vs stratégie aléatoire
- **ROI annuel :** XXX-XXX% selon scénarios
- **Validation :** Basé sur analyse XXX+ films réels

---

## 📁 Structure du Projet
