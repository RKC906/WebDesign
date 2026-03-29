# WebDesign
projet de web design en binome, site d'informations sur la guerre en Iran

## Environnement Docker (PHP + Apache + MySQL)

### Services disponibles
- FrontOffice (PHP/Apache) : http://localhost:8080
- BackOffice (PHP/Apache) : http://localhost:8081
- MySQL 8.4 : localhost:3306

### Démarrage
1. Copier les variables d'environnement :
	- `cp .env.example .env`
2. Lancer les conteneurs :
	- `docker compose up -d --build`
3. Vérifier les logs si besoin :
	- `docker compose logs -f`

### Base de données
- Un script d'initialisation est chargé automatiquement au premier démarrage :
  - `docker/mysql/init/00-schema.sql`
- Base créée : `webdesign`
- Utilisateur par défaut : `webdesign` / `webdesign`

### Arrêt
- `docker compose down`
