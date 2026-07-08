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
| Plunging Strike | ↓ + X in the air — dive blade-first; bounces you higher than a jump off a kill. Hold ↓ to pogo-chain |
| Hurl fire | C / L *(once Brand banks the heat — Act II)* |
| Start  | Enter · Pause P · Music M |

Touch controls appear on mobile.

## Act I — The Ash Harvest

March east through razed Caldermark: the farmhouse with the meal still on the
table, the burned scarecrow pointing the way, the dead orchard, the mill still
turning with one sail aflame. Eight screens, ending at a shrine where one stone
is still warm.

![The Ash Harvest](screenshots/field.png)

- **The horde:** Bone Levies (fodder), Ash Hounds (they charge — jump or cut),
  Iron Brigands (three hits; bait the telegraphed axe and punish)
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

Acts II (The Cold Hearth) and III (The Hungry Light) — with the Warden's Coal,
fireballs from the blade, Ember Cultists, Cinder Wraiths, and Selwyn the Warm —
are speced in [STORYBOARD.md](STORYBOARD.md) and coming next.

## Under the hood

- Vanilla JS on one `<canvas>`, fixed 60fps timestep
- **Procedural pixel sprites**: painted shaded regions, auto-outlined, dither
  textured — the hero has 5 poses × 4 transformation stages, all generated
- Game-feel per a design consult: 4-frame hitstop, 9 on crits, weighted crit odds
  with a pity timer, particle and shake budgets, corpse physics
- WebAudio synth for everything: somber D-minor loop, crit ring-outs, chain
  pitch escalation
- The story is told in set dressing — look closely at the shrines' lantern
  brackets
