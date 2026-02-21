# La Guerra di Valle Aurelia

A browser-based beat-em-up about **Daniele "il Conte"** fighting the gang of Valle Aurelia across the streets of Prati, Rome.

Built with pure HTML5 Canvas + JavaScript. No dependencies. Single file.

## How to Play

Open `index.html` in any browser (Chrome, Firefox, Safari, Edge). No installation needed. Mobile touch controls are supported.

### Difficulty

Choose at game start:

| Difficulty | Lives | Damage Taken | Enemy HP |
|------------|-------|--------------|----------|
| **Easy** | Infinite | -30% | -20% |
| **Medium** | 3 per boss | Normal | Normal |
| **Hard** | 3 total (no resets) | +10% | +10% |

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
| S | Open shop — Armeria di Giammy e Mele (at hub) |
| B | Open casino — Bingo degli Ubaldi (at Vanni hub) |
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

Pick one of 4 starter weapons at game start. Upgrade at Giammy & Mele's shop, or spin La Ruota (gacha) for rare/legendary weapons.

| Weapon | Type | Style |
|--------|------|-------|
| Sanpietrino | Starter | Fast 4-hit combo, crit scales with chain |
| Cacciavite | Starter | Always bleeds on hit, Ultra boosts bleed |
| Spranga | Starter | Heavy, long range, high poise, double hit |
| Fionda | Starter | Ranged slingshot, 3rd hit pierces (Ultra only) |
| Machete | Rare (gacha) | Ultra: 2x damage on enemies below 25% HP |
| Catena | Rare (gacha) | Always AoE, Ultra pulls enemies in |
| Bottiglia Rotta | Rare (gacha) | Very fast, high crit, Ultra bleeds |
| La Lupa | Legendary (gacha) | The she-wolf blade, Ultra shockwave |
| Pistola del Nonno | Legendary (gacha) | Ranged, all shots pierce |
| Manganello | Secret | Michele's police baton — Ultra slows all enemies |

### Helpers

Unlock helpers as you progress. Each has a cooldown and 3 upgrade tiers (bought at the shop):

- **Pirox** — DJ scratch that stuns nearby enemies
- **Tommy** — Throws a knife in a drunken arc
- **Cicca** — Heals you (it's a cat)
- **Il Mostro** — Speed boost aura

### Casino — Bingo degli Ubaldi

Press **B** from the hub (Vanni's Bar) to enter the casino. Two mini-games are available:

| Game | NPC | Rules |
|------|-----|-------|
| **Video Poker** (Jacks or Better) | Andreino Volpi | Deal 5 cards, hold the ones you want, draw replacements. Jacks or Better pays 1x up to Royal Flush at 250x. Bet 5-100 coins. |
| **Slot Machine** | Panda | Spin 3 reels. Three-of-a-kind pays big, pairs pay small. Bet 5-50 coins. |

Casino controls:

| Key | Action |
|-----|--------|
| B (from hub) | Open casino |
| ESC | Return to hub |
| 1 / 2 | Switch tab (Poker / Slots) |
| Left/Right | Adjust bet |
| Enter | Deal / Draw / Spin |
| 1-5 (poker hold phase) | Toggle hold on cards |

NPCs:
- **Andreino Volpi** — Poker-obsessed ex-footballer with a PokerStars hat, bad knee, and a joint. Comments on your hands.
- **Panda** — A panda obsessed with padel and tennis. Works sports references into everything.

### Secret Codes

Type these on the credits screen:

| Code | Effect |
|------|--------|
| `CONTE` | Unlock everything — all weapons, max upgrades, all helpers tier 3 |
| `LUDO` | +100 coins |
| `FREE` | Play the Cicca & Daniele freestyle music video |
| `YO` | Toggle sunglasses on Daniele (persists for the whole run) |

### Hub Secrets

The hub hides interactive secrets -- click/tap to discover them:

- Punch the street lamp for bonus coins (once per run)
- Pet Cicca the cat when she wanders by
- Tap the left wall of Vanni's bar repeatedly
- Try the drink at the outdoor table for a combat buff
- Click the front door of Bar Vanni to find Michele Lo Sbirro's backroom -- choose wisely and you may receive the Manganello (police baton) weapon whose Ultra slows all enemies

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

- Single `index.html` file (~10800 lines)
- HTML5 Canvas (900x550) with responsive scaling
- Web Audio API synthesizer for music (no audio files)
- Mobile touch controls with virtual buttons
- No frameworks, no build step, no dependencies
