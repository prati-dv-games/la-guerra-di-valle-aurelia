# La Guerra di Valle Aurelia

A browser-based beat-em-up about **Daniele "il Conte"** fighting the gang of Valle Aurelia across the streets of Prati, Rome.

Built with pure HTML5 Canvas + JavaScript. No dependencies. Single file.

## How to Play

Open `index.html` in any browser (Chrome, Firefox, Safari, Edge). No installation needed. Mobile touch controls are supported.

### Difficulty

Choose at game start:

| Difficulty | Lives | Damage Taken | Enemy HP |
|------------|-------|--------------|----------|
| **Easy** | Infinite | 60% | 70% |
| **Medium** | 3 per boss | 100% | 100% |
| **Hard** | 3 total (no resets) | 100% | 100% |

### Controls

| Key | Action |
|-----|--------|
| A/D or Arrow Left/Right | Move |
| W or Arrow Up | Jump |
| Z or Space | Attack (combo chains) |
| X | Dodge (invincibility frames) |
| C | Use consumable |
| V | Ultra attack (when bar is full) |
| 1 | Helper: Pirox (DJ stun) |
| 2 | Helper: Tommy (drunk knife) |
| 3 | Helper: Cicca the cat (heal) |
| 4 | Helper: Il Mostro (speed boost) |
| S | Open shop (at Vanni hub) |
| M | Mute/unmute music |
| ESC | Back / return to hub |

On mobile, on-screen touch buttons replace keyboard controls.

### Playing on PS5

The game supports the DualSense controller via the Gamepad API. Since the PS5 browser can't open local files, you need to host the game online first (see "How to Share" below), then navigate to the URL in the PS5's built-in browser.

| DualSense | Action |
|-----------|--------|
| Left Stick / D-pad | Move |
| Triangle | Jump |
| Cross (X) | Attack / Confirm |
| Circle (O) | Dodge |
| Square | Ultra (when bar is full) |
| L1 / R1 | Helper 1 (Pirox) / Helper 2 (Tommy) |
| L2 / R2 | Helper 3 (Cicca) / Helper 4 (Il Mostro) |
| L3 / R3 | Use consumable |
| Options | Pause / Back |
| Create | Moves screen |

Use the touchpad as a mouse for hub menus and the shop. Any standard gamepad (Xbox, Switch Pro, etc.) also works with the same layout.

### Combat System

- **Combo chains**: chain attacks together; timing the next hit in the combo window keeps the chain going
- **Dodge**: invincibility frames, builds dodge counter for bonus damage
- **Ultra**: fills by dealing damage; press V when full for a powerful attack
- **Consumables**: buy from the shop, use mid-fight for heals or buffs
- **Chain multiplier**: consecutive hits without getting hit increase damage output

### Bosses

1. **LaFed** (Via Plava) — Vain rugby guy, raps mid-fight
2. **Gioacchino** (Down Under Pub) — Baton attacks + sister Regina throws meat
3. **Il Dale** (Piazza Bainsizza) — Tall and dumb, hits hard
4. **Ciccio Ruver** (Pizzarium) — Mohawk pizza maker, summons minions
5. **Pisellino** (Piazza Mazzini) — Final boss on a moped + uncle Mariuso

### Weapons

Buy weapons at the Vanni shop between levels:

| Weapon | Style |
|--------|-------|
| Pugni | Starting fists |
| Sanpietrino | Fast 4-hit combo, crit scales with chain |
| Bastone | Balanced stick |
| Bottiglia Rotta | Glass bottle, bleeds on crit |
| Machete | Slow but heavy damage |
| Catena | Chain with wide range |
| Pistola | Ranged |
| La Lupa | Legendary — the she-wolf blade |

### Helpers

Unlock helpers as you progress. Each has a cooldown and 3 upgrade tiers (bought at the shop):

- **Pirox** — DJ scratch that stuns nearby enemies
- **Tommy** — Throws a knife in a drunken arc
- **Cicca** — Heals you (it's a cat)
- **Il Mostro** — Speed boost aura

### Secret Codes

Type these on the credits screen:

| Code | Effect |
|------|--------|
| `CONTE` | Unlock everything — all weapons, max upgrades, all helpers tier 3 |
| `FREESTYLE` | Play the Cicca & Daniele freestyle music video |

## How to Share

### Option 1: Send the file directly
Send `index.html` (+ `prati_freestyle.mp4` for the video) via WhatsApp, Telegram, or email. Open in browser. Done.

### Option 2: Netlify Drop
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag the `la-guerra-di-valle-aurelia` folder onto the page
3. Get a shareable URL

### Option 3: GitHub Pages
1. Push to a GitHub repository
2. Settings > Pages > Source: main branch
3. Game lives at `https://<user>.github.io/la-guerra-di-valle-aurelia/`

## Tech

- Single `index.html` file (~9500 lines)
- HTML5 Canvas (900x550) with responsive scaling
- Web Audio API synthesizer for music (no audio files)
- Mobile touch controls with virtual buttons
- No frameworks, no build step, no dependencies
