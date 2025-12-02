# Groovarr Requirements

## Vision

Groovarr extends the *-arr* ecosystem to Plex music playlists.  

It enables users to:

- Create new playlists or add to existing ones.
- Fetch tracks from online sources (MusicBrainz, Spotify, YouTube Music).
- Directly sync playlists to Plex or export/import them offline (M3U, JSON, CSV).

---

## Functional Requirements

- **Playlist Management**
  - Create, edit, delete playlists.
  - Link playlists to Plex libraries.
- **Track Management**
  - Search tracks from online sources.
  - Add/remove tracks in playlists.
- **Import/Export**
  - Export playlists in M3U format (initial).
  - Import playlists from M3U files.
  - Future: JSON/CSV formats.
- **Plex Integration**
  - Authenticate with Plex token.
  - Create/update Plex playlists.
  - Append tracks to existing Plex playlists.
- **UI**
  - Web-based interface for playlist creation and track search.
  - Minimal MVP UI with React + Vite.

---

## Non-Functional Requirements

- **Cross-platform:** Must run on Linux and Windows.
- **API-first:** REST endpoints with Swagger/OpenAPI.
- **Extensibility:** Modular services for sources, Plex, import/export.
- **Persistence:** In-memory for MVP; SQLite/PostgreSQL for production.
- **Logging:** Structured logging with Serilog.
- **Background Jobs:** Scheduled syncs with Quartz.NET.

---

## Development Tool Stack

### Backend

- **Language:** C# with .NET 8 (ASP.NET Core Web API).
- **Persistence:** EF Core with SQLite (MVP), PostgreSQL (production).
- **Logging:** Serilog.
- **Jobs:** Quartz.NET for scheduled tasks.

### Frontend

- **Framework:** React + Vite (TypeScript).
- **API Client:** Axios.
- **Styling:** TailwindCSS or Material UI.

### Tooling

- **IDE:** Visual Studio Code (Linux/Win)
- **Build:** `dotnet CLI` (`dotnet build`, `dotnet run`).
- **Testing:** xUnit/NUnit (backend), Jest (frontend).
- **API Debugging:** Swagger/OpenAPI.
- **Version Control:** Git + GitHub.
- **Containers:** Docker/Docker Compose.
- **CI/CD:** GitHub Actions (Linux + Windows runners).
