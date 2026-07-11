# 🔥 EMBERWARD

*A Tale of Caldermark* — a gritty retro side-scroller in a single HTML file.
No build step, no dependencies, no assets. Open it and play.

> When Caldermark's own Hearth-Warden stopped tending the King's Coal and let it
> feed on him, the fire that had warmed a kingdom walked out its gates and ate it.
> One knight survived, hearthless, with an empty lantern and a sword named Brand.

![Title](screenshots/title.png)

## Play

Open `index.html` in any modern browser, or serve it:

```
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Controls

| Action | Keys |
|--------|------|
| Move   | ← → or A / D |
| Jump   | ↑ / W / Space / Z (hold for height) |
| Sword  | X / J / K |
| Rising Strike | hold jump + X on the ground — leap with an upward cut |
| Skyward Cut | ↑ + X — slash overhead, standing or mid-jump; the answer to anything above you |
| Plunging Strike | ↓ + X in the air — dive blade-first; bounces you higher than a jump off a kill. Hold ↓ to pogo-chain |
| Hurl fire | C / L *(once Brand banks the heat at the Cold Hearth)* |
| Start  | Enter · Pause P · Music M |

On mobile a gamepad appears: a d-pad under the left thumb (slide for
diagonals — ▲/▼ are the strike modifiers) and jump / strike face buttons
under the right, joined by a 🔥 button once Brand banks the heat.

## Act I — The Ash Harvest

March east through razed Caldermark: the farmhouse with the meal still on the
table, the burned scarecrow pointing the way, the dead orchard, the mill still
turning with one sail aflame. Eight screens, ending at a shrine where one stone
is still warm.

![The Ash Harvest](screenshots/field.png)

- **The horde:** Bone Levies (fodder), Ash Hounds (big ash-grey farm dogs that
  spring into a charge — jump or cut), Ash Imps (small, erratic hoppers — worth
  double a levy if you can hit one), Iron Brigands (three hits; bait the
  telegraphed swing — and at range they hurl spinning axes you can bat out of
  the air). No two beasts patrol at quite the same tempo.
- **The Blade Catches:** find the soldier's fire-steel and one strike in twenty
  turns your foe to ash
- **Tending:** checkpoints are torches you light — `TENDED.` refills everything
- **Kill chains** (DOUBLE! TRIPLE! RAMPAGE!), corpse-launch kill pops, hitstop,
  and a quiet HUD: ember-diamond hearts, three coals in the lantern, XP
- **Aerial combat pays**: airborne kills earn +50% XP, and the plunge pogo-chains
  through packs — dive perches are built over the campfire arena for exactly that
- **The high road pays**: a 3-jump chain to a warm ember above the scarecrow
  field, a skyway over the ravine, treetop coin tiers, secret braziers to slash
  alight
- **SPARK:** enough XP and the hero visibly transforms — slow-mo, converging
  embers, a shockwave — first stage of Spark → Kindled → Ablaze
- **Grade card** at the act's end: time, the fallen, coals spent, best chain → D–S

## Act II — The Cold Hearth

The castle the fire walked out of, under a bone moon. Eight screens: the
gatehouse doors torn *outward*, the roofless great hall, the stripped armory
with floors that give way underfoot, the spiral stair, and the Cold Hearth
itself — where the game quietly explains the empty lantern, and Brand drinks
the Warden's Coal.

![The Great Hall](screenshots/act2-hall.png)

- **Cinder Wraiths** float out of sword reach and swoop — the Skyward Cut and
  Rising Strike are their answer
- **Ember Cultists** lob fire from ledges; hurl fire back, or parry the lob
  out of the air with a slash
- **The Warden's Coal:** fireballs open Brigands, pierce fodder, and light
  braziers the sword can't reach; 5 sword hits bank an ember, checkpoints
  refill the blade
- **Traps:** collapsing floors, swinging censers over pits
- The twist is stated exactly once, at the kneeling-stone. Watch the far
  rampart from the broken east wall.

![The Cold Hearth](screenshots/act2-hearth.png)

Act III (The Hungry Light) — the war camp, the full-roster gauntlet, and
Selwyn the Warm — is speced in [STORYBOARD.md](STORYBOARD.md) and coming next.

## Under the hood

- Vanilla JS on one `<canvas>`, fixed 60fps timestep
- **Procedural pixel sprites**: painted shaded regions, auto-outlined, dither
  textured — the hero has 5 poses × 4 transformation stages, all generated
- Game-feel per a design consult: 4-frame hitstop, 9 on crits, weighted crit odds
  with a pity timer, particle and shake budgets, corpse physics
- WebAudio synth for everything, with an **adaptive score** (designed with an
  8/16-bit chiptune consult): the somber D-minor base loop never changes, but
  each transformation stage adds a layer — a heartbeat at SPARK, a rolling
  arpeggio at KINDLED, an octave gallop with drums at ABLAZE — and Act II
  moves the whole song to G minor over a lament bass with a dead chapel bell.
  Crit ring-outs, chain pitch escalation
- The story is told in set dressing — look closely at the shrines' lantern
  brackets
