# Website

Landingpage von Stagecraft Solutions unter `stagecraft.solutions`.

**Stand:** Platzhalterseite. Die eigentliche Seite kommt später.

## Betrieb (Hermes)

- Adresse: `stagecraft.solutions` → DSM-Reverse-Proxy → `127.0.0.1:8752`
- Der Container läuft über die gemeinsame `docker-compose.yml` in `/volume1/docker/StagecraftSolutions` (Dienst `website`).
- Inhalt liegt in `public/` (statisch, nginx).
- Aktualisieren: dort `./update.sh website` (holt `main` per `git pull` und baut neu).
