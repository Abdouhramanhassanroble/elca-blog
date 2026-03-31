# ELCA Blog

Blog tech propulsé par Drupal 10, thème Twig custom et composant React.
Conçu pour partager les bonnes pratiques du développement web moderne
dans l'univers des agences digitales.

## Stack

- Drupal 10 — CMS back-end
- MySQL 8 — Base de données
- Twig — Thème custom responsive Mobile-first
- React 18 — Composant front-end branché sur JSON:API Drupal
- Docker Compose — Environnement local reproductible
- GitLab CI — Pipeline CI/CD automatisé

## Lancer le projet en local

### Prérequis
- Docker Desktop installé et lancé

### Installation

1. Cloner le repo
   git clone https://github.com/ton-username/elca-blog.git
   cd elca-blog

2. Lancer les containers
   docker compose up -d

3. Ouvrir localhost:8080 et suivre l'installation Drupal
   - Database host     : db
   - Database name     : drupal
   - Database user     : drupal
   - Database password : drupal

4. Activer le thème custom
   localhost:8080/admin/appearance → ELCA Blog → Install and set as default

5. Si le CSS ne s'affiche pas
   localhost:8080/admin/config/development/performance → Clear all caches

## Structure

themes/custom/elcablog/     → Thème Twig custom responsive
modules/custom/             → Modules custom

## Bugs rencontrés et solutions

- Docker volumes sur lecteur E: → déplacer le projet sur C:
- CSS manquant → trusted_host_patterns + preprocess_page
- URLs propres → a2enmod rewrite déjà actif, routing via /?q=

## Auteur

Abdouhraman Hassan