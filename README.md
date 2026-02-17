# cc-ecosystem-registry

Zentrale Registry fuer Claude Code Skills, MCP-Server und Templates.

## Format

Die `registry.json` folgt dem Schema v2.0.0. Jede Komponente hat:

| Feld | Beschreibung |
|------|-------------|
| `id` | Eindeutige ID im Format `{typ}-{owner}-{name}` |
| `type` | `skill`, `mcp` oder `template` |
| `owner` | `own` (privat), `community` (oeffentlich) oder `local` (kein Repo) |
| `name` | Anzeigename |
| `description` | Kurzbeschreibung |
| `path` | Relativer Pfad in der Registry |
| `git` | Git-Repo-Informationen (oder null) |
| `tags` | Suchbare Tags |
| `status` | `active`, `planned` oder `deprecated` |
| `install` | Installationsdetails (Dateien, Runtime, Post-Install) |
| `requires` | Abhaengigkeiten (Env-Vars, Runtimes) |

## Verwendung

Diese Registry wird vom Claude Code Terminal Profile Setup automatisch geladen.
Siehe: [Claude-Terminal-Profile](https://github.com/Wagner-Emden-IT-Services/Claude-Terminal-Profile)
