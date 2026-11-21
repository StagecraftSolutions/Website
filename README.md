# Website

Landingpage von Stagecraft Solutions unter `stagecraft.solutions`.

**Stand:** Landingpage mit Hero, Kennzahlen, Ablauf, Prüfungen der Rack Manufaktur, den drei Projekten, offenen Daten, FAQ, Impressum und Datenschutz. Noch `noindex`.

Lokal ansehen: `python3 -m http.server 8771 -d public`, dann <http://localhost:8771/>. Keine externen Quellen; Schriften (OFL 1.1) und Bilder liegen in `public/assets/`.

## Betrieb (Hermes)

- Adresse: `stagecraft.solutions` → DSM-Reverse-Proxy → `127.0.0.1:8752`
- Der Container läuft über die gemeinsame `docker-compose.yml` in `/volume1/docker/StagecraftSolutions` (Dienst `website`).
- Inhalt liegt in `public/` (statisch, nginx).
- Aktualisieren: dort `./update.sh website` (holt `main` per `git pull` und baut neu).
