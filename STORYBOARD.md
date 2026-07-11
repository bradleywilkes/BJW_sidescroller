# EMBERWARD — Storyboard & Build Spec (v2)

*A Tale of Caldermark. Developed across three rounds with a fantasy-writing story
consultant, plus a game-feel/engagement consult with a game-design specialist,
and an 8/16-bit chiptune consult for the adaptive score.*

**Build status:** Acts I and II are playable end to end. Act III and the Selwyn
fight are next.

---

## The theme: TWO FIRES

**The fire that warms and the fire that consumes are one and the same. The difference is a keeper.**

A hearth is fire that is kept, fed carefully, shared. A wildfire is fire that keeps
itself. The villain didn't bring fire to the kingdom — he *was its fire-keeper*, and
he stopped tending and started feeding. The hero is the last man still tending:
every torch he lights, every checkpoint he plants, is the theme in one button-press.

The hero and the villain are the only two figures in the world with ember-glow
behind their visors. The player levels up by feeding their own inner fire — and
watches their own sprite transform toward the villain's condition all game long.

## The names

| Thing | Name | Why |
|---|---|---|
| The game | **EMBERWARD** (*A Tale of Caldermark*) | *-ward* = keeping/tending; the theme in one word |
| The kingdom | **Caldermark** | sounds like a real place on an old map, not a fantasy-name generator |
| The hero | **The Knight of the Cold Hearth** | named for the hearth he was denied — a fault he wrongly carries as his own until the Act II reveal |
| The villain | **Selwyn** (Old English *sele* + *wine*: "hall-friend") | a kindly steward's name — the Ember Warden's job description fossilized. The hall's friend is what ended the hall. Menace is 100% context |
| His epithet | "the Unquenched" survives only as what the **cultists** call him | his own boss card is titled "the Warm" instead — the menace comes from the warmth (see the intro card below) |
| The sword | **Brand** | Old English/Norse: both "sword" and "burning log" |
| Bone Footman | **Bone Levy** | Caldermark's own conscripted dead |

Boss intro card:

> `SELWYN THE WARM`
> `He kept your fire. He keeps it still.`

"He keeps it still" is the whole villain: in his mind the theft is continued duty.

## The premise

When the Ember Warden of Caldermark stopped tending the King's hearth and let it
feed on him, the fire that had warmed a kingdom walked out its gates and consumed it.
One knight survived, blaming himself for the hearth gone cold, with an empty
lantern and a sword named Brand.
He marches east through the ash to take back the stolen fire — and decide, at the
gate of the man it hollowed, whether it should ever be lit again.

Title screen press line: `PRESS ENTER TO KEEP THE FLAME`

**The premise crawl** (3 cards after START, before Act I — the game tells its own
premise instead of leaving it to the README):

> `The King's Coal warmed all Caldermark.` / `Its Warden was sworn to tend it.`
> `He stopped. It fed on him instead.` / `Then it fed on the kingdom.`
> `One knight lived. His lantern, empty.` / `He marches east to take back the fire.`

## THE TWIST — The Denied Succession

*(The hero's tragedy. Never stated in Act I; it drips.)*

The Ember Warden's office passes by lantern: when a Warden's watch ends, he fills
his successor's lantern from the King's Coal and steps down. **The hero was the
chosen successor.** He knelt at the great hearth with his empty lantern — and
Selwyn refused to pass the fire. Refused to let his watch end. He fed the Coal
instead of handing it on; it fed on him, and then on Caldermark.

**The empty lantern the player carries from screen one was never emptied by
tragedy — it was never filled.** Not revenge: *inheritance withheld.*

**The drip:**

- **Act I (plant, no text).** Every roadside shrine has two iron lantern-brackets —
  one always empty. Reads as looting now, ritual later. Checkpoint idle animation:
  the hero lifts his lantern to the lit torch for a beat, then lowers it, still dark.
  Players notice by the third checkpoint. Nothing is explained.
- **Act II-5, the Cold Hearth (reveal).** Beside the great hearth: the Warden's iron
  mantle in the ash — and a kneeling-stone with a lantern cradle. The hero's lantern
  clicks in perfectly. Two cards, poetry then plain fact (the only place the
  mechanism is stated — review flagged that the twist's causal fact must reach
  the player somewhere):
  `The lantern fits the cradle.` / `It was never filled.`
  `A Warden fills his heir's lantern.` / `Selwyn never let his watch end.`
  Then the Warden's Coal — the succession finally happens, wrong way round: by
  salvage, not rite, and into the *sword*, not the lantern.
- **Act III (recontextualize).** Cultist graffiti: soot-paintings of lanterns crossed
  out — the cult are failed aspirants who begged Selwyn for fire, were refused, and
  chose to feed rather than carry. The field of dark visors (III-6) lands twice:
  everyone in this war was denied the fire except the man hoarding it. A fire
  hoarded *is* a wildfire.
- **Epilogue (cards unchanged, now heavier).** **Kindle** = the hero completes his
  own denied investiture — takes up the watch that destroys its keepers, while his
  sprite already burns Ablaze. `Tended, this time.` becomes a vow. **Refuse** = he
  ends the succession itself — the one thing Selwyn could never do.
  `No fire outlives its keeper twice.` becomes doctrine.

---

## Systems

### Health
- Hero: 3 hearts → 5 via **Hearthstones** (end of Act I, mid Act III). Heart refills
  are **embers**; healing is literally being warmed.
- Enemies: Bone Levy 1 hit · Ash Hound 1 · Ash Imp 1 (small erratic hopper,
  premium XP) · Cinder Wraith 1 · Ember Cultist 2 · Iron Brigand 3 (telegraphed
  heavy swing; hurls a parryable axe at range) · Selwyn: 3 phases.
  Every spawn rolls its own patrol tempo so packs don't march in lockstep.

### Fireball — "Embers in the Blade"
At the Cold Hearth, Brand drinks the Warden's Coal: heat banked in steel. Each
throw visibly un-banks the blade — edge-glow shortens toward the hilt. On the last
charge Brand goes ash-black; it still cuts. *(The sword is not its fire; the man is
not his.)*

- **Max 3 Embers**, shown as flame pips on the sword in the HUD + blade edge-glow.
- **Recharge:** 5 sword hits = 1 Ember. **Crits bank a full Ember instantly.**
- **Checkpoints refill fully** (tending gives) — this also kills hoarding: banking
  past a checkpoint has zero value.
- At 3/3, sword hits spill wasted sparks + fizzle SFX — the blade is begging.
- Fireball damage 2 (the sword does 1): it opens the 3-hit Brigand, sword finishes. Pierces
  fodder, stops on heavies. Projectile 5.0 px/f, slight droop (gravity 0.06).
  Cast: 16f total (6f raise + glow, release, 10f recovery), grounded-only.
- Flyers and lobbers perch out of sword reach — the fireball's obvious prey.
- Toast: `A kept coal. Brand banks the heat.` Empty-blade flash: `BRAND RUNS COLD`
- **Secret braziers** (~5 per act, some fireball-only) upgrade max Embers 3→4→5.

### Crits — "The Blade Catches"
Brand means both sword and burning log — one strike in twenty, the blade catches
like kindling. No dice anywhere.

- Flash line: `THE BLADE CATCHES` — Brand's edge goes white-hot for a frame with a
  spark spray; the struck enemy flares to a black ash-silhouette before crumbling.
- Odds weighted where they're felt: 1-in-20 on fodder, 1-in-12 on Brigand/boss.
  Pity timer: guaranteed after 24 non-crits; after a crit, next 3 hits can't.
- Damage 2× ("a free fireball"), 9f hitstop (normal 4), 14-spark cone, +5 semitone
  ring-out SFX, 2px directional shake.
- The fiction is taught by the **Soldier's Fire-Steel** pickup (Act I-7): a
  flint-and-striker found in a horde campfire pit, so the crit reads as flint
  striking steel rather than a dice roll.
  Toast: `A soldier's fire-steel. Struck true.`

### Leveling — visible transformation (Spark → Kindled → Ablaze)
Each stage moves the hero's silhouette toward Selwyn's:

- **SPARK:** visor glow flicker → steady; faint hot line along Brand's edge;
  2-3 ember particles trail him at a run.
- **KINDLED:** cape hem chars and glows, shedding sparks on jumps; ember-orange
  cracks open at the armor *joints* — the exact seam-glow the player will later see
  on Selwyn in boss phase 2; visor brightens a palette step.
- **ABLAZE:** the crimson crest burns like a torch flame; ember cracks spread across
  the chestplate mirroring Selwyn's phase 1; the visor casts actual light in dark
  rooms (gameplay-legible in the keep and epilogue).
- By Ablaze the hero's palette reads closer to the boss's than to his own Act I
  sprite. The player should quietly wonder how much of the man is left to burn.

**The transformation moment (showstopper, no cutscene, ~2s, control never taken):**
game speed lerps to 25% over 20 real frames → screen darkens 40% except the hero →
30 ember particles converge *inward* over 45 frames → 3-frame white flash, palette
swap → shockwave ring (~200px) kills fodder and staggers heavies → speed snaps back
with 6f hitstop and a synth swell. Level layouts place a trash pack near expected
level-up points — the shockwave needs victims.

Toasts: `SPARK. THE EMBER STIRS.` · `KINDLED. THE VISOR BRIGHTENS.` ·
`ABLAZE. HOW BRIGHTLY YOU BURN.`

### Lives, checkpoints, coins
Three coals in the lantern; each death spends one (`One coal spent.`). Checkpoints
are torches/banners the hero lights and plants — dark → lit on use (`TENDED.`), and
they refill hearts context and Embers. Coins are dead men's coins, tallied into XP.

---

## ACT I — THE ASH HARVEST

> `The wind carried it east.`
> `So he walked east.`

| # | Visual beat | Gameplay beat |
|---|---|---|
| 1 | Farmhouse door open; table set, meal cold | No enemies. Walk + tutorial jump; first checkpoint torch |
| 2 | Scarecrow burned to its post, one arm pointing east | **Bone Levy** intro ×2 |
| 3 | Dead orchard; embers drift through branches like blossom; a shrine with two lantern-brackets, one empty | **Ash Hound** intro, charging from off-screen; treetop coin line |
| 4 | Farm well, ropes burnt through; a dog's collar beside it | Levies + Hound mixed; first heart-ember after the fight |
| 5 | Mill with one sail burning, still slowly turning | Rooftop platforming; a Cinder Wraith crosses the background sky — teased only |
| 6 | Abandoned refugee cart, toys spilled on the road; second bracket-shrine | **Iron Brigand** intro blocking the road; teaches telegraph-dodge. Checkpoint |
| 7 | Horde campfire pit: bones, kingdom coins, a dead soldier's fire-steel in the ash | Wave fight; **Soldier's Fire-Steel** pickup (crits unlock) |
| 8 | Roadside shrine, cache looted, one stone still warm | Mini-gauntlet; **Hearthstone** (4th heart); **SPARK** transformation lands |

## ACT II — THE COLD HEARTH

> `Every hearth in Caldermark was lit`
> `from one fire. He knew where it lived.`

| # | Visual beat | Gameplay beat |
|---|---|---|
| 1 | Gatehouse doors torn *outward* — the fire left; nothing broke in | Rubble-climb intro; Levies on the stairs |
| 2 | Great hall roofless; sky where rafters were | **Cinder Wraith** true intro, swooping between beam-hops |
| 3 | Armory racks stripped bare but for one child-sized helm | Brigands in a tight corridor; collapsing-floor trap |
| 4 | Spiral stair; arrow-slit light shafts full of ember-drift | Zigzag platform climb — the game's tallest, spanning the full screen height — with Wraiths diving through the shafts; mid-climb checkpoint |
| 5 | **THE COLD HEARTH** — arena-sized dead hearth; the Warden's iron mantle in the ash; a kneeling-stone with a lantern cradle | Silent screen, no enemies. Lantern-cradle card (the twist reveal), then **Warden's Coal** — Brand ignites; fireball tutorial on unlit braziers |
| 6 | Hearth-sigils painted inverted in soot — cultist graffiti | **Ember Cultist** intro lobbing fire from ledges; fireball is the counter-tool. First cultist kill toast: `They tithe to a nameless warmth.` |
| 7 | Throne room; the throne alone untouched and dustless | Trap gauntlet — swinging censers, spike pits — into an ambush wave |
| 8 | Broken east wall framing the war camp's glow — and on a distant rampart in that glow, one small ember-lit silhouette. Selwyn, seen once, far off | Long descent, mixed gauntlet; **KINDLED** transformation; checkpoint |

## ACT III — THE HUNGRY LIGHT

> `His camp burned brighter than the kingdom.`
> `Nothing in it was warm.`

| # | Visual beat | Gameplay beat |
|---|---|---|
| 1 | Palisade built from the scorched house-doors of Caldermark homes | Bright firelight now hostile; Cultists + Hounds together |
| 2 | Cage wagons, all empty, doors open — nothing kept, everything fed | Brigand pairs; fire trenches to leap |
| 3 | Tithe-brazier ringed with offered gauntlets — hands and all; crossed-out lantern graffiti | Cultist nest wave; heart-embers scarce from here on |
| 4 | Mound of Caldermark's crimson banners piled for burning | **Hearthstone** (5th heart) hidden behind the mound; checkpoint |
| 5 | Horde forge melting kingdom coins into cleaver steel | Bellows-and-spark platforming; Wraiths in the smoke |
| 6 | Ranked horde helms on posts — every visor dark. Only two visors in this world glow | Full-roster gauntlet |
| 7 | Avenue of torches taller than houses; the hero's visor-glow vanishes against the blaze | No enemies. A dread walk. Final checkpoint. Silence is the beat |
| 8 | Arena: a bonfire of banners, Selwyn feeding it by hand | **BOSS**; **ABLAZE** reached during the fight |

## The boss — SELWYN THE WARM

> `SELWYN THE WARM`
> `He kept your fire. He keeps it still.`

1. **The Warden** — slow, telegraphed cleaver arcs, a keeper's discipline guarding
   the coal in his chest; the man he was still holds the line.
2. **The Untended** — armor seams crack and vent (the same seam-glow the player
   wears since Kindled); he ignites floor patches he then avoids feeding — the fire
   is escaping him; faster but sloppier.
3. **The Wildfire** — cleaver dropped half-melted; a walking bonfire doing
   Ash-Hound rushes as the arena edges ignite. **He brightens as his HP drops:**
   dying as pure spending.

Phase transitions: 20f hitstop, white flash, palette shift hotter, 8px shake over
30f, arena torches flare. **Death beat — no text.** He gutters; the fire leaves him
standing, then the husk falls. Every light dies except the King's Coal glowing
where he stood. Darkest screen in the game.

## Epilogue (playable, silent)

At the dead great hearth, coal in hand. As the hero approaches, he instinctively
begins the lantern-lift gesture he has performed at every checkpoint — then stops
himself mid-motion, lantern raised, awaiting input. That one held frame is the
tell that this moment is a decision. Press attack to kindle — or walk off-screen
to refuse. No prompt, no menu.

**Act III checkpoint idle**: the familiar lantern-lift gains a half-second
hesitation before he does it — fire feels different here. (The mechanical hinge
of the Act III inversion, taught through the animation the player has seen 15+
times.)

- **KINDLE:** `The great hearth of Caldermark burned.` / `Tended, this time.`
- **REFUSE:** `He left the coal to the cold.` / `No fire outlives its keeper twice.`

---

## Combat feel & engagement (from the game-design consult)

**Priority order:** melee hitstop → kill pop → fireball economy → crit recipe →
transformation → kill chains → grade cards.

- **Hitstop:** 4f on every sword contact (9f crits; 20f boss phase breaks). Only on
  flesh contact — never on whiffs, pickups, or projectile launches.
- **Kill pop:** corpse flashes white 2f, launches 45° away (vx ±3.5, vy −5),
  spins off-screen; 8 particles; `+XP` popup. Death louder than damage.
- **Slash arc flash:** 3-frame white crescent at the sword tip.
- **Kill chains:** kills within 90f chain — SFX pitch climbs +2 semitones per link
  (cap +8), popups `DOUBLE!` / `TRIPLE!` / `RAMPAGE!`; a 3-chain banks a bonus Ember.
- **Last-heart tension:** at 1 hp the crest flame gutters, music ducks −6dB, slow
  heartbeat. Comebacks become stories.
- **Player pain is quiet:** short low thud, 2f red flash, small shake. Fireworks are
  for what the player *does*, not what's done to them. Respawn under 1.5s.
- **End-of-act grade cards:** time / kills / deaths / secrets / best chain → D–S
  grade, stamped with a thunk and 6f hitstop. Instant replay goals.
- **NG+ "Ashen Knight"** (post-clear): start Ablaze with 5 Embers, 2 max hearts,
  remixed enemy placement, visible speedrun timer.
- **Discipline caps:** shake only for damage-taken/crits/boss/transformation, summed
  and clamped ≤8px; ≤60 live particles (≤16 per event); no damage numbers on normal
  hits; popup text only for crits, chains, +XP, +HP.

## All in-game text

| Moment | Line |
|---|---|
| Press start | `PRESS START TO KEEP THE FLAME` |
| Coin | `A dead man's coin. Carry it home.` |
| Heart ember | `An ember. It warms what it can.` |
| Hearthstone | `A hearthstone, still warm. Keep it.` |
| Warden's Coal | `A kept coal. Brand banks the heat.` |
| Fire-Steel | `A soldier's fire-steel. Struck true.` |
| Crit flash | `THE BLADE CATCHES` |
| Fireball empty | `BRAND RUNS COLD` |
| Checkpoint | `TENDED.` |
| Twist card (II-5) | `The lantern fits the cradle.` / `It was never filled.` |
| Level 1 | `SPARK. THE EMBER STIRS.` |
| Level 2 | `KINDLED. THE VISOR BRIGHTENS.` |
| Level 3 | `ABLAZE. HOW BRIGHTLY YOU BURN.` |
| Death | `One coal spent.` |
| Game over | `The lantern is empty.` / `The wind takes the rest.` |
| Boss intro | `SELWYN THE WARM` / `He kept your fire. He keeps it still.` |
| Tally header | `HOW BRIGHTLY DID YOU BURN?` |

## Enemy lore (bestiary lines)

- **Ash Hound** — *The farm dogs stayed by the burned homes. The fire kept them.*
- **Ash Imp** — *Something small learned to love the ash.*
- **Bone Levy** — *The kingdom's levy still musters. For the other side.*
- **Iron Brigand** — *Sellswords paid in dead men's coin. They will be paid again.*
- **Cinder Wraith** — *It rose as smoke and never came down.*
- **Ember Cultist** — *They tithe their flesh to the one they call Unquenched. He had a name once.*

## The toy (human-scale thread)

A small carved crimson toy appears three times, no text ever: on the farmhouse
doorstep in I-1, among the spilled toys at the refugee cart in I-6, and in the
horde's tithe-pile in III-3. Whether the farm was *his* home is never said.

## Motif checklist (visual rules for the build)

1. **Warm light = tended/safe** through Acts I–II; **Act III inverts it**. III-7 is the hinge.
2. **Only three things glow ember-orange:** the hero (visor, and spreading with each
   level), Selwyn, and kept fires. No decorative orange anywhere else.
3. **The hero transforms per level** (Spark/Kindled/Ablaze sprite swaps) — each stage
   borrows a visual element the player will later recognize on Selwyn.
4. **Two fire languages:** tended fire small, round, steady, slow-animated; wildfire
   tall, ragged, fast-animated. Never mix the sprite sets.
5. **Checkpoints change state on use:** dark torch/furled banner → lit + planted.
   The hero's idle there: lifts his lantern to the flame, lowers it, still dark.
6. **Enemy visors and eye-slits are always dark** — pays off at III-6.
7. **Ember-drift always blows left-to-right** (the wind went east).
8. **Selwyn brightens as his HP drops;** after his death, the darkest palette in the
   game — the King's Coal the only warmth left.
9. **Paired lantern-brackets on every shrine, one always empty** — the twist,
   hiding in set dressing from screen 3.
