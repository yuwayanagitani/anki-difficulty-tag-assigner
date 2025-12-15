# Anki Difficulty Tagger

AnkiWeb: https://ankiweb.net/shared/by-author/2117859718

This Anki add-on automatically assigns a 5-level difficulty tag to notes based on review statistics (lapses, interval, ease), so you can quickly filter cards by how difficult they are in practice.

## Features
- Assigns difficulty tags (e.g. difficulty:1 — difficulty:5) based on review history
- Configurable thresholds and tag names
- Works without modifying card templates — tags are added to notes
- Run ad-hoc from the Tools menu or schedule batch updates

## Installation
1. Open Anki → Tools → Add-ons → Open Add-ons Folder.
2. Clone or copy this add-on's folder into the add-ons directory (e.g. `addons21/anki-difficulty-tagger`).
3. Restart Anki.

## Usage
- Tools → Difficulty Tagger → Run on selected notes / all notes.
- Tags are added to notes; use the Browser to filter, search, and edit as needed.

## Configuration
Edit `config.json` in the add-on folder to tune:
- thresholds for difficulties
- tag base name (default: `difficulty`)
- whether to remove old difficulty tags before assignment

Example (partial):
```json
{
  "tag_base": "difficulty",
  "thresholds": [0.2, 0.4, 0.6, 0.8]
}
```

## Development
- The add-on is written in Python for Anki's add-on API.
- Run linting/tests locally and restart Anki to load changes.

## Issues & Support
Report issues or feature requests in this repository's Issues. Include Anki version and steps to reproduce.

## License
See LICENSE file for license information.
