# La Guerra di Valle Aurelia — Project Instructions

## Architecture

- **Single-file game**: everything lives in `index.html` (~9500 lines of JS inside a `<script>` tag)
- **Canvas**: 900x550, scaled responsively to viewport
- **Music**: Web Audio API oscillator-based synthesizer, no audio files
- **Video**: `prati_freestyle.mp4` — freestyle music video by Cicca & Daniele

## Syntax Check

After any code change, always verify:

```bash
sed -n '/<script>/,/<\/script>/p' index.html | sed '1d;$d' > /tmp/check.js && node -c /tmp/check.js
```

## README Maintenance

**Proactively update `README.md`** whenever a change materially affects what a player or contributor would need to know. This includes:

- New game mechanics, weapons, helpers, or bosses
- Changes to controls or key bindings
- New cheat codes or secret features
- Difficulty system changes
- New files added to the project (assets, etc.)
- Sharing/hosting instructions if they change

Do NOT update the README for:
- Internal refactors, performance fixes, or bug fixes that don't change player-facing behavior
- Minor tuning (damage numbers, cooldown tweaks, visual polish)

Keep the README concise and scannable. Use tables for structured info. No emojis.
