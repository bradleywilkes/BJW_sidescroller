# EMBERWARD — Storyboard & Build Spec

*A Tale of Caldermark. Developed with a fantasy-writing story consult, two rounds.*

---

## The theme: TWO FIRES

**The fire that warms and the fire that eats are the same fire. Tending is the whole moral question.**

A hearth is fire that is kept, fed carefully, shared. A wildfire is fire that keeps
itself. The villain didn't bring fire to the kingdom — he *was its fire-keeper*, and
he stopped tending and started feeding. The hero is the last man still tending:
every torch he lights, every checkpoint he plants, is the theme in one button-press.

The hero and the villain are the only two figures in the world with ember-glow
behind their visors. The player levels up by feeding their own inner fire — and
watches their visor brighten toward Grimald's condition all game long.

## The names

| Was | Is now | Why |
|---|---|---|
| Emberwood Quest | **EMBERWARD** (*A Tale of Caldermark*) | *-ward* = keeping/tending; the theme in one word |
| the kingdom | **Caldermark** | reads found, not generated |
| the hero | **The Hearthless Knight** | defined by what he lost custody of |
| Warlord Vargul | **Grimald the Unquenched** | once Hearth-Warden of Caldermark, keeper of the King's Coal; he fed it until it consumed him |
| the sword | **Brand** | Old English/Norse: means both "sword" and "burning log" |
| Bone Footman | **Bone Levy** | these are Caldermark's own conscripted dead |

**Premise.** When Caldermark's own Hearth-Warden stopped tending the King's Coal
and let it feed on him, he became Grimald the Unquenched, and the fire that had
warmed a kingdom walked out its gates and ate it. One knight survived, hearthless,
with an empty lantern and a sword named Brand. He marches east through the ash to
do the only thing a keeper of fires can still do: take back the stolen coal — and
decide, at the gate of the man it hollowed, whether it should ever be lit again.

Title screen press line: `PRESS START TO KEEP THE FLAME`

---

## Systems (the owner's asks, grounded in the story)

- **Health.** Hero starts at 3 hearts, upgradeable to 5 via **Hearthstones**
  (stones from home fires, still warm) — one at the end of Act I, one mid-Act III.
  Heart refills are **embers** dropped in the world. Healing is literally being warmed.
- **Enemy health tiers.** Bone Levy 1 hit (fodder, as requested) · Ash Hound 1 ·
  Cinder Wraith 1 · Ember Cultist 2 · Iron Brigand 3 with a telegraphed heavy
  swing · Grimald: 3 phases.
- **Fireball powerup.** The **Warden's Coal**, found mid-Act II at the Cold Hearth
  itself. The hero feeds it into his empty lantern; Brand ignites; attack gains a
  thrown hearth-fire projectile. Toast: `A kept coal. Brand takes the light.`
- **Leveling.** XP (kills + coins) levels the hero: **SPARK → KINDLED → ABLAZE**,
  landing roughly at each act's end. Each level visibly brightens the visor glow
  and adds a small power bump (details in build: +damage reach at Kindled,
  +fireball size at Ablaze). Tally screen: `HOW BRIGHTLY DID YOU BURN?`
- **d20 crits.** The **Soldier's Bone**, a carved d20 knucklebone looted from a
  horde campfire in Act I — from then on kills roll the die on screen; nat 20
  flashes `THE DEAD THROW WITH YOU`.
- **Lives & checkpoints.** Three coals in the lantern; each death spends one
  (`One coal spent.`). Checkpoints are torches/banners the hero lights and
  plants — dark → lit on use. Toast: `TENDED.`
- **Coins** are dead men's coins, tallied into XP: the fire fed by what's carried.

---

## ACT I — THE ASH HARVEST

> `The wind carried it east.`
> `So he walked east.`

| # | Visual beat | Gameplay beat |
|---|---|---|
| 1 | Farmhouse door open; table set, meal cold | No enemies. Walk + tutorial jump; first checkpoint torch (`TENDED.`) |
| 2 | Scarecrow burned to its post, one arm pointing east | **Bone Levy** intro ×2; one-hit kills showcase the d20 flash |
| 3 | Dead orchard; embers drift through branches like blossom | **Ash Hound** intro, charging from off-screen; coin line in the treetops |
| 4 | Farm well, ropes burnt through; a dog's collar beside it | Levies + Hound mixed; first heart-ember after the fight |
| 5 | Mill with one sail burning, still slowly turning | Rooftop platforming; a Cinder Wraith crosses the background sky — teased only |
| 6 | Abandoned refugee cart, toys spilled on the road | **Iron Brigand** intro blocking the road; teaches telegraph-dodge. Checkpoint |
| 7 | Horde campfire pit: bones, kingdom coins, carved dice in the ash | Wave fight; **Soldier's Bone** pickup |
| 8 | Roadside shrine, cache looted, one stone still warm | Mini-gauntlet; **Hearthstone** (4th heart); **SPARK** level lands |

## ACT II — THE COLD HEARTH

> `Every hearth in Caldermark was lit`
> `from one fire. He knew where it lived.`

| # | Visual beat | Gameplay beat |
|---|---|---|
| 1 | Gatehouse doors torn *outward* — the fire left; nothing broke in | Rubble-climb intro; Levies on the stairs |
| 2 | Great hall roofless; sky where rafters were | **Cinder Wraith** true intro, swooping between beam-hops |
| 3 | Armory racks stripped bare but for one child-sized helm | Brigands in a tight corridor; collapsing-floor trap |
| 4 | Spiral stair; arrow-slit light shafts full of ember-drift | Vertical climb, Wraiths diving through the shafts; mid-climb checkpoint |
| 5 | **THE COLD HEARTH** — arena-sized dead hearth; the Warden's abandoned iron mantle in the ash | Silent screen, no enemies. **Warden's Coal** pickup — Brand ignites; fireball tutorial on a chain of unlit braziers |
| 6 | Hearth-sigils painted inverted in soot — cultist graffiti | **Ember Cultist** intro lobbing fire from ledges; fireball is the counter-tool |
| 7 | Throne room; the throne alone untouched and dustless | Trap gauntlet — swinging censers, spike pits — into an ambush wave |
| 8 | Broken east wall framing the war camp's glow on the horizon | Long descent, mixed gauntlet; **KINDLED** level lands; checkpoint |

## ACT III — THE HUNGRY LIGHT

> `His camp burned brighter than the kingdom.`
> `Nothing in it was warm.`

| # | Visual beat | Gameplay beat |
|---|---|---|
| 1 | Palisade built from the scorched house-doors of Caldermark homes | Bright firelight now hostile; Cultists + Hounds together |
| 2 | Cage wagons, all empty, doors open — nothing kept, everything fed | Brigand pairs; fire trenches to leap |
| 3 | Tithe-brazier ringed with gauntlets the cultists offered — hands and all | Cultist nest wave; heart-embers scarce from here on |
| 4 | Mound of Caldermark's crimson banners piled for burning | **Hearthstone** (5th heart) hidden behind the mound; checkpoint |
| 5 | Horde forge melting kingdom coins into cleaver steel | Bellows-and-spark platforming; Wraiths in the smoke |
| 6 | Ranked horde helms on posts — every visor dark. Only two visors in this world glow | Full-roster gauntlet |
| 7 | Avenue of torches taller than houses; the hero's visor-glow vanishes against the blaze | No enemies. A dread walk. Final checkpoint. Silence is the beat |
| 8 | Arena: a bonfire of banners, Grimald feeding it by hand | **BOSS**; **ABLAZE** reached during the fight |

## The boss — GRIMALD THE UNQUENCHED

> `GRIMALD THE UNQUENCHED`
> `Once, he kept your fire.`

1. **The Warden** — slow, telegraphed cleaver arcs, a keeper's discipline guarding
   the coal in his chest; the man he was still holds the line.
2. **The Untended** — armor seams crack and vent; he ignites floor patches he then
   avoids feeding — the fire is escaping him; faster but sloppier.
3. **The Wildfire** — cleaver dropped half-melted; a walking bonfire doing
   Ash-Hound rushes as the arena edges ignite. The brighter his sprite burns,
   the lower his health: dying as pure spending.

**Death beat — no text.** He gutters; the fire leaves him standing, then the husk
falls. Every light in the arena dies except the **King's Coal** glowing where he
stood. Darkest screen in the game.

## Epilogue (playable, silent)

At the dead great hearth, coal in hand. Walk to the hearth and press attack to
kindle it — or walk off-screen to refuse. No prompt tells the player this.

- **KINDLE:** `The great hearth of Caldermark burned.` / `Tended, this time.`
- **REFUSE:** `He left the coal to the cold.` / `No fire outlives its keeper twice.`

## All in-game text (fits retro budgets)

| Moment | Line |
|---|---|
| Coin | `A dead man's coin. Carry it home.` |
| Heart ember | `An ember. It warms what it can.` |
| Hearthstone | `A hearthstone, still warm. Keep it.` |
| Warden's Coal | `A kept coal. Brand takes the light.` |
| Soldier's Bone | `A carved bone die. The dead ante up.` |
| Nat-20 flash | `THE DEAD THROW WITH YOU` |
| Checkpoint | `TENDED.` |
| Level 1 | `SPARK. THE EMBER STIRS.` |
| Level 2 | `KINDLED. THE VISOR BRIGHTENS.` |
| Level 3 | `ABLAZE. HOW BRIGHTLY YOU BURN.` |
| Death | `One coal spent.` |
| Game over | `The lantern is empty.` / `The wind takes the rest.` |
| Tally header | `HOW BRIGHTLY DID YOU BURN?` |

## Enemy lore (bestiary lines)

- **Ash Hound** — *The farm dogs stayed by the burned homes. The fire kept them.*
- **Bone Levy** — *The kingdom's levy still musters. For the other side.*
- **Iron Brigand** — *Sellswords paid in dead men's coin. They will be paid again.*
- **Cinder Wraith** — *What rises with the smoke does not settle with the ash.*
- **Ember Cultist** — *They tithe their own flesh to the Unquenched, and call the hunger holy.*

## Motif checklist (visual rules for the build)

1. **Warm light = tended/safe** through Acts I–II; **Act III inverts it** — firelight
   means threat, darkness means rest. Screen III-7 is the hinge.
2. **Only three things glow ember-orange:** the hero's visor, Grimald, and kept
   fires (checkpoints, hearths). No decorative orange glows anywhere else.
3. **Hero's visor brightens per level** (Spark/Kindled/Ablaze sprite swaps).
4. **Two fire languages:** tended fire is small, round, steady, slow-animated;
   wildfire is tall, ragged, fast-animated. Never mix the sprite sets.
5. **Checkpoints change state on use:** dark torch/furled banner → lit torch +
   planted banner. Every save is an act of tending.
6. **Enemy visors and eye-slits are always dark** — pays off at III-6 and makes
   the Grimald mirror land.
7. **Ember-drift always blows left-to-right** (the wind went east) — ambient
   particles double as direction language.
8. **Grimald brightens as his HP drops;** after his death, cut to the darkest
   palette in the game so the King's Coal reads as the only warmth left.
