# esMauricie
Dépôt du rapport de recherche en science des données sur l'état de l'économie sociale en Mauricie

## Contexte et problématique  
Le Pôle d’économie sociale de la Mauricie vise à **doubler son nombre de membres** en 2025–2026 pour atteindre **150 adhérents**.
Pour soutenir cette croissance, il est essentiel d’orienter stratégiquement les démarches de recrutement en identifiant les zones de sous-représentation sur le territoire de la Mauricie.  

## Objectifs  
1. **Cartographier** l’ensemble du territoire administratif 04 (MRC et municipalités).
2. **Intégrer** et **consolider** les données internes du Pôle (annuaire, répertoire AirTable) et les sources externes (REQ, ISQ, MRNF) pour produire un **tableau de bord**.  

## Sources de données  
| Source                                     | Type et rôle                                                   |
|--------------------------------------------|---------------------------------------------------------------|
| Pôle d’économie sociale de la Mauricie     | CSV (MemberPress : liste des membres) et AirTable (répertoire)|
| Registre des entreprises du Québec (REQ)   | CSV : liste des entreprises actives (filtrage RA04 & formes ES) (juin 2025) |
| MRNF                                       | Shapefiles : limites administratives de la Mauricie (MRC)     |
| Institut de la statistique du Québec (ISQ) | Indicateurs sociodémographiques par MRC                       |
| Répertoire des municipalités du Québec     | CSV : inventaire complet des municipalités                    |


## Structure du dépôt 

├── data/                       # Jeux de données bruts
│   ├── Pôle/                   # Données internes du Pôle d’économie sociale
│   ├── REQ/                    # Fichiers du Registre des entreprises du Québec
│   ├── SHP/                    # Shapefiles (limites administratives)
│   └── MUN.csv                 # Inventaire des municipalités
├── site_dashboard/             # Code du dashboard interactif
│   ├── images/                 # Images pour le dashboard
│   ├── index.qmd               # Quarto source du dashboard
│   └── styles.css              # Styles personnalisés
├── site_data/                  # Site statique de présentation des données
│   ├── images/                 # Visuels et cartes pour le site de données
│   ├── _quarto.yml             # Configuration Quarto du site de données
│   ├── index.qmd               # Page d’accueil du site de données
│   ├── pole.qmd                # Traitement des données du Pôle d’économie sociale
│   ├── req.qmd                 # Traitement des données du Registre des entreprises
│   ├── references.qmd          # Bibliographie et références
│   └── styles.css              # Styles personnalisés
└── references.bib 				# Fichier BibTeX pour la bibliographie