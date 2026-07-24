# Unraid templates for Budgero

Community Apps templates for [Budgero](https://budgero.app/) — a source-available, end-to-end encrypted zero-based budgeting app. These templates are MIT-licensed; Budgero itself is licensed under [FSL-1.1-ALv2](https://github.com/tombadilo-bombadilo/budgero/blob/master/LICENSE).

## Install

Once accepted into Community Apps, search for **Budgero** in the Apps tab.

Until then, add this repo manually: **Docker tab → Template Repositories** → add
`https://github.com/tombadilo-bombadilo/unraid-templates` → **Add Container** → pick the Budgero template.

## Configuration

| Setting | Default | Notes |
| --- | --- | --- |
| WebUI Port | `3001` | Web UI and sync WebSocket |
| Data | `/mnt/user/appdata/budgero` | SQLite database and app data |
| Allowed sync origins | — | **Required.** Exact origin you open the app from, e.g. `http://192.168.1.50:3001`. Comma-separated for multiple. No wildcards — sync is rejected from unlisted origins and the budget will not load. |

## Support

Bugs and questions: [GitHub Issues](https://github.com/tombadilo-bombadilo/budgero/issues) · Self-host docs: [budgero.app/self-hostable](https://budgero.app/self-hostable)
