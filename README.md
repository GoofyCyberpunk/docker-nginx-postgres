# docker-nginx-postgres
Docker Compose setup with nginx and PostgreSQL containers

Projekt abgeschlossen – Ziel war es, zu lernen, wie man mit Docker Compose 
mehrere zusammenhängende Container (Webserver + Datenbank) gemeinsam verwaltet.

## Docker Compose Setup

- docker-compose.yml erstellt mit zwei Services: nginx (Webserver) + PostgreSQL (Datenbank)
- `docker compose up` startet beide Container gemeinsam aus einer einzigen Konfigurationsdatei
- Ports: nginx auf 8080 (Host) → 80 (Container), PostgreSQL auf 5432
- Beide Container laufen unabhängig, aber koordiniert über docker-compose
- Verifiziert mit `docker ps`: beide Container laufen stabil im Hintergrund