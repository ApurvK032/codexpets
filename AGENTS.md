# CodexPets

## Project Purpose
Explore and prototype custom Codex pets: visual companion avatars shown by the Codex app/extension pet overlay.

## Tech Stack
Plain Markdown docs plus pet manifest examples for now. Custom Codex pets are folder-based manifests plus sprite sheets.

## Setup / Run / Test
- Run local Pixelorama: `.\tools\Pixelorama-v1.1.10\Pixelorama-Windows-64bit\Pixelorama.exe`
- No automated tests yet.

## Important Files
- `AGENTS.md`: durable project guidance for future Codex sessions.
- `AGENT_LOG.md`: optional dated session notes when useful.
- `README.md`: beginner guide for real Codex pet structure.
- `templates/pet.json`: manifest template for a custom pet.
- `templates/spritesheet-layout.md`: required sprite sheet dimensions and animation rows.
- `art/spark/`: current Spark pet draft with an original demo sprite sheet and guide.
- `assets/preview/`: repo-owned README preview GIFs/frame strips generated from Spark.
- `pets/`: design notes or draft pet assets before copying into `%USERPROFILE%\.codex\pets`.
- `tools/`: local downloaded tooling, ignored by git.

## Coding Conventions
- Prefer small, focused edits.
- Keep docs concise and practical.
- Custom pets should be staged as one folder per pet, with `pet.json` and a `spritesheet.webp` or `spritesheet.png`.
- The sprite sheet must be exactly `1536x1872`, arranged as `8` columns by `9` rows of `192x208` frames.

## Known Issues
- Custom pet support was observed in a local Codex extension build and may change as Codex updates.
- Custom pet folder is `%USERPROFILE%\.codex\pets`.
- Built-in pet sprite sheets were observed under `%USERPROFILE%\.vscode\extensions\openai.chatgpt-26.429.30905-win32-x64\webview\assets` as `codex`, `dewey`, `fireball`, `rocky`, `seedy`, `stacky`, `bsod`, and `null-signal` WebP files.
- `art/spark/spritesheet.png` is an original demo `1536x1872` Spark sprite sheet.
- GitHub remote target: `https://github.com/ApurvK032/codexpets`.

## Workflow Expectations
- Read this file before planning or editing.
- Update this file when durable project knowledge changes.
- Use `AGENT_LOG.md` for important dated work notes, not as a long transcript.
- For OpenAI or Codex feature claims, verify against official OpenAI docs or the OpenAI docs MCP server.
