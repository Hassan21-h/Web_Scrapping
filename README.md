# Quotes Scraper & Analyzer

Projet de web scraping et d'analyse de données bibliographiques développé en Python.

## Description
Ce projet collecte l'intégralité des citations, des tags associés et des fiches biographiques d'auteurs à partir d'un site cible, puis effectue une analyse statistique simple des fréquences.

## Fonctionnalités
- **Conformité** : Vérification du fichier `robots.txt` avant toute requête.
- **Scraping optimisé** : Extraction des citations paginées et dédoublonnage des requêtes vers les fiches auteurs.
- **Analyse** : Structuration dans Pandas (`DataFrame`), extraction du **Top 5 auteurs** et **Top 10 tags**.

## Structure des données générées
- `citations_completes` : Citations nettoyées avec URLs, tags sous forme de listes et informations complètes sur l'auteur.
- `top_auteurs` / `top_tags` : Classements triés par fréquence décroissante.

## Prérequis
- Python 3.8+
- Bibliothèques : `requests`, `beautifulsoup4`, `pandas`

```bash
pip install requests beautifulsoup4 pandas