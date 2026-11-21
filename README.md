# Website

Landingpage von Stagecraft Solutions unter `stagecraft.solutions`.

**Stand:** Platzhalterseite. Die eigentliche Seite kommt später.

## Betrieb (Hermes)

- Adresse: `stagecraft.solutions` → DSM-Reverse-Proxy → `127.0.0.1:8752`
- Inhalt liegt in `public/` (statisch, nginx).
- Starten/aktualisieren:

  ```bash
  git pull && docker compose up -d --build
  ```
