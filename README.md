# Aurora Addon Library

Curated catalog of legal Stremio addons. Consumed by the Aurora Android TV app.

- **Edit** `addons.json` via the GitHub web UI.
- App fetches via jsDelivr CDN: `https://cdn.jsdelivr.net/gh/Pwn5ince94/aurora-addons@main/addons.json`
- The app silently falls back to its built-in 3-entry catalog if this file is unreachable or malformed.

## Schema

```json
{
  "version": 1,
  "addons": [
    {
      "id": "unique-slug",
      "name": "Display Name",
      "description": "One-line description",
      "manifestUrl": "https://addon/manifest.json",
      "category": "metadata | subtitles | catalog | sync",
      "developer": "Optional",
      "official": true,
      "featured": false
    }
  ]
}
```
