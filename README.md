# PocketBase (LazyCat LPK)

Single-file backend: SQLite + auth + file storage + admin UI + REST API.

- Upstream: https://github.com/pocketbase/pocketbase
- Image: ghcr.io/muchobien/pocketbase:0.40.6 (mirror mode, digest-matched)
- License: MIT (full text in content/licenses/LICENSE)
- Containers: single (SQLite under /pb_data)

## Notes

- **Image comes from ghcr.io**, not Docker Hub. This validates that the Action can
  authenticate and mirror GHCR-hosted images (earlier exclusions of GHCR-only apps
  were overly cautious).
- No seeded account: the first admin is created by visiting the /_/ admin UI.
- All state (SQLite db, uploads) lives in /lzcapp/var/pb_data.
- No mail service configured.
- Not yet verified on a real device.
