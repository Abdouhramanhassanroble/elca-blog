# DrivePress

Blog headless propulsé par Drupal 10, thème Twig custom et composant React.

Projet de démonstration — Candidature Développeur Web / CMS / Front-End Junior.

## Stack

- Drupal 10 — CMS back-end
- MySQL 8 — Base de données
- Twig — Thème custom responsive
- React 18 — Composant front-end branché sur l'API JSON:API Drupal
- Docker Compose — Environnement local

## Lancer le projet en local

### Prérequis
- Docker Desktop installé et lancé

### Installation

1. Cloner le repo
   git clone https://github.com/ton-username/drivepress.git
   cd drivepress

2. Lancer les containers
   docker compose up -d

3. Ouvrir localhost:8080 et suivre l'installation Drupal
   - Database host : db
   - Database name : drupal
   - Database user : drupal
   - Database password : drupal

4. Vider le cache si le CSS ne s'affiche pas
   localhost:8080/admin/config/development/performance

## Structure

themes/custom/drivepress/   → Thème Twig custom
modules/custom/             → Modules custom (à venir)

## Auteur

Abdouhraman Hassan