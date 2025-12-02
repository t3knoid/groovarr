# Groovarr Roadmap

## Roadmap

### Milestone 1 — Minimum Viable Product(MVP)

- Scaffold backend (ASP.NET Core API).
- Scaffold frontend (React + Vite).
- In-memory playlist storage.
- Stubbed source fetch service.
- M3U export/import.
- Swagger docs.
- CI/CD build scripts

### Milestone 2 — Plex Sync

- Implement PlexService with real API calls.
- Support playlist create/update/append in Plex.
- Add UI toggle for direct Plex sync vs offline export.

### Milestone 3 — Persistence

- Integrate EF Core with SQLite.
- Add migrations.
- Optionally support PostgreSQL for production.

### Milestone 4 — Source Adapters

- Implement MusicBrainz adapter.
- Add Spotify and YouTube Music adapters.
- Unified interface for source fetchers.

### Milestone 5 — CI/CD

- GitHub Actions pipeline:
  - Build/test backend on Linux + Windows runners.
  - Build/test frontend.
- Automated releases with tagged builds.

### Milestone 6 — Advanced Features

- JSON/CSV import/export formats.
- Background sync jobs (Quartz.NET).
- Authentication (API keys or OAuth).
- Monitoring (Prometheus/Grafana).
- Reverse proxy (Nginx/Caddy) for production.

---

## Success Criteria

- Runs identically on Linux and Windows (via Docker or native).
- Aligns with *-arr* ecosystem conventions (C#, modular services, REST API).
- Provides a usable MVP for Plex playlist management.
- Extensible for future sources and formats.
