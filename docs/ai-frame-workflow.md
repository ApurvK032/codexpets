# AI Frame Workflow

AI image tools can help create raw animation frames, but Codex needs one exact sprite sheet.

## Recommended Flow

1. Generate a clean character reference first.
2. Generate one animation strip at a time, such as `running-right`.
3. Ask for a flat removable background color, like magenta `#ff00ff`.
4. Crop each frame individually.
5. Remove the background.
6. Fit each character into a transparent `192x208` frame.
7. Paste the frames into the correct row of the `1536x1872` sprite sheet.

## Animation Rows

| Row | State | Frames |
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

## Prompt Starter

```text
Create an 8-frame horizontal pixel-art sprite strip of the same small robot character running to the right.
Use consistent proportions, consistent colors, and no labels.
Place each pose evenly spaced on a flat #ff00ff background.
Use crisp pixel art, transparent-ready edges, and no shadows.
```

After generation, the strip still needs to be sliced and assembled into the real Codex pet sprite sheet.
