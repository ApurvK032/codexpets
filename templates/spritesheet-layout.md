# Codex Pet Sprite Sheet Layout

Custom Codex pets use one PNG or WebP sprite sheet.

## Required Size

- Image size: `1536x1872`
- Columns: `8`
- Rows: `9`
- Frame size: `192x208`

## Row Map

| Row | State | Frames Used |
| --- | --- | --- |
| 0 | idle | 6 |
| 1 | running-right | 8 |
| 2 | running-left | 8 |
| 3 | waving | 4 |
| 4 | jumping | 5 |
| 5 | failed | 8 |
| 6 | waiting | 6 |
| 7 | running | 6 |
| 8 | review | 6 |

Unused cells should still exist in the sheet. They can be duplicates or blank transparent frames.

## Manifest

Place a `pet.json` file next to the sprite sheet:

```json
{
  "displayName": "My Pet",
  "description": "A short line shown in the Codex pet picker.",
  "spritesheetPath": "spritesheet.webp"
}
```

The `spritesheetPath` must point to a file inside the same pet folder.
