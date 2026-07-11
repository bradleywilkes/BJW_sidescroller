# EMBERWARD — Storyboard & Build Spec (v3)

*A Tale of Caldermark. Developed across three rounds with a fantasy-writing story
consultant, plus a game-feel/engagement consult with a game-design specialist,
an 8/16-bit chiptune consult for the adaptive score, and a v3 narrative revamp
centering the hero's redemption arc.*

**Build status:** Acts I and II are playable end to end. Act III, the Selwyn
fight, and the epilogue are speced here and not yet built.

---

## The theme: TWO FIRES

**The fire that warms and the fire that consumes are one and the same. The difference is a keeper.**

A hearth is fire that is kept, fed carefully, shared. A wildfire is fire that keeps
itself. The villain didn't bring fire to the kingdom — he *was its fire-keeper*, and
he stopped tending and started feeding. The hero is the last man still tending:
every torch he lights, every checkpoint he plants, is the theme in one button-press.

v3 sharpens the second reading of the tagline: *the difference is a keeper* is also
a question — who decides who gets to keep? The hero has spent the whole march
believing the fire itself judged him and found him unworthy of the watch. The truth
is that fire doesn't judge; keepers do — and the keeper lied. **This is a redemption
story, and the redemption is not earning the fire. It is learning he was never the
one who failed.**

The hero and the villain are the only two figures in the world with ember-glow
behind their visors. The player levels up by feeding their own inner fire — and
watches their own sprite transform toward the villain's condition all game long.

## The names

| Thing | Name | Why |
|---|---|---|
| The game | **EMBERWARD** (*A Tale of Caldermark*) | *-ward* = keeping/tending; the theme in one word — and the office the game is named for |
| The kingdom | **Caldermark** | sounds like a real place on an old map, not a fantasy-name generator |
| The office | **the Ember Warden of Caldermark** | the crown's fire-keeper, sworn to tend the King's Ember. Full title on first reference; "the Warden" alone after |
| The fire | **the King's Ember** | the seed-fire every hearth in Caldermark was lit from. It lives in the King's hearth — the hearth is the place, the Ember is the fire in it |
| The salvage | **the Warden's Coal** | keeps its name: a coal is a piece raked from a fire and carried; the Ember is the living fire itself. What Brand drinks at the Cold Hearth is a carried piece, not the flame |
| The hero | **the Knight of the Cold Hearth** | named for the hearth he was denied — a fault he wrongly carries as his own until the Act II reveal |
| The villain | **Selwyn** (Old English *sele* + *wine*: "hall-friend") | a kindly steward's name — the Ember Warden's job description fossilized. The hall's friend is what ended the hall. Menace is 100% context |
| His epithet | "the Unquenched" survives only as what the **cultists** call him | his own boss card is titled "the Warm" instead — the menace comes from the warmth (see the intro card below) |
| The sword | **Brand** | Old English/Norse: both "sword" and "burning log" |
| Bone Footman | **Bone Levy** | Caldermark's own conscripted dead |

Boss intro card:

> `SELWYN THE WARM`
> `He kept your fire. He keeps it still.`

"He keeps it still" is the whole villain: in his mind the theft is continued duty.
And after the Act II reveal the line turns a second time — *your* fire is literal.
It was the hero's inheritance to receive, and Selwyn kept it.

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

> `The King's Ember warmed all Caldermark.` / `Its Ember Warden was sworn to tend it.`
> `He stopped. It fed on him instead.` / `Then it fed on the kingdom.`
> `One knight lived, and blamed himself.` / `He marches east to take back the fire.`

Card three is the self-blame plant: the game states the hero carries fault before
it says anything else about him — and never says for what. The Cold Hearth answers.

## THE TWIST — The Withheld Fire

*(The hero's tragedy — and, he will learn, never his fault. Never stated in Act I;
it drips.)*

The Ember Warden's office passes by lantern: when a Warden's watch ends, he kneels
his heir at the great hearth and fills the heir's lantern from the King's Ember.
But that is not what aspirants are taught. The doctrine of the rite says *the
Warden lifts the lantern, and the Ember chooses* — an old, convenient lie that
lets a passed-over aspirant blame the fire instead of the man.

**The hero was the chosen heir.** He knelt at the great hearth. Selwyn performed
the rite in full — raised the empty lantern to the King's Ember, held it there,
lowered it dark. The court read the fire's judgment. The hero read his own
unworthiness, and he has carried it ever since: he believes the hearth went cold
because the Ember weighed him and found nothing worth passing on.

The truth: the Ember does not choose. A Warden *fills* his heir's lantern — an act
of will, a gift given. Selwyn withheld it. He never intended to let his watch end —
not for this heir, not for any. He performed the rite as theater, let the shame
land on the kneeling man, and went on feeding the Ember instead of handing it on;
it fed on him, and then on Caldermark.

**The empty lantern the player carries from screen one was never emptied by
tragedy — it was never filled.** And the fault the hero carries from card three of
the crawl was never his — it was manufactured. Not revenge: *inheritance withheld,
and the blame for it planted on the heir.*

**The reveal must land twice** — this is the load-bearing craft note for II-5. The
*player* learns the succession mechanism and that the hero was the heir. The *hero*
learns that the rite is a gift, not a judgment: the fire never refused him — a man
did. Both revelations ride the same two cards.

**The drip:**

- **Crawl card three (plant, one line).** `One knight lived, and blamed himself.`
  The fault is stated before the quest is — and never explained until II-5.
- **Act I (plant, no text).** Every roadside shrine has two iron lantern-brackets —
  one always empty. Reads as looting now, ritual later. Checkpoint idle animation:
  the hero lifts his lantern to the lit torch for a beat, then lowers it, still
  dark. This is not habit — it is the rite, re-asked. At every fire he tends he
  offers his lantern again, and takes its darkness as the same answer. The player
  is watching a man confirm his own sentence twenty times over. Nothing is
  explained. Players notice by the third checkpoint.
- **Act II-5, the Cold Hearth (reveal).** Beside the great hearth: the Warden's iron
  mantle in the ash — and a kneeling-stone with a lantern cradle. The hero's lantern
  clicks in perfectly. Two cards, poetry then plain fact (the only place the
  mechanism is stated — the twist's causal fact must reach the player here):
  `The lantern fits the cradle.` / `It was never filled.`
  `A Warden fills his heir's lantern.` / `Selwyn never let his watch end.`
  Dual reading, card by card: the first card is the *player's* — the cradle proves
  he was the heir, and *never filled* means never emptied by loss. The second card
  is the *hero's* — a Warden **fills** the lantern; filling is the Warden's act,
  not the Ember's verdict. The fire never judged him. The refusal was a man's,
  wearing the fire's face. `Selwyn never let his watch end.` names the wrong out
  loud.
  Then the Warden's Coal — the succession finally happens, wrong way round: by
  salvage, not rite, and into the *sword*, not the lantern. He takes the
  inheritance the only way left to take it.
- **Act III (dark mirror).** The cult are failed aspirants — people who knelt
  somewhere down the years, watched their lanterns stay dark, and believed the same
  lie the hero believed. He kept tending anyway; they chose to feed. Crossed-out
  lantern soot-graffiti, the Aspirants' Wall (III-3), and one kneeling cultist
  performing the hero's own checkpoint ceremony. The field of dark visors (III-6)
  lands twice: everyone in this war was told the fire refused them — and only the
  man hoarding it knew it never chooses. A fire hoarded *is* a wildfire.
- **Epilogue (same cards, new weight).** Whichever ending the player picks, it is
  chosen by a man who now knows the fault was never his — unworthiness has left the
  room. **Kindle** = he completes the investiture that was stolen from him, eyes
  open about what the watch does to its keepers. `Tended, this time.` is a vow.
  **Refuse** = he lets the watch end — the one thing Selwyn could never do.
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
  (The redemption answer, delivered by the epilogue: what's left is the keeper.)

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
they refill hearts and Embers. Coins are dead men's coins, tallied into XP.

---

## ACT I — THE ASH HARVEST *(built)*

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

## ACT II — THE COLD HEARTH *(built)*

> `Every hearth in Caldermark was lit`
> `from one fire. He knew where it lived.`

| # | Visual beat | Gameplay beat |
|---|---|---|
| 1 | Gatehouse doors torn *outward* — the fire left; nothing broke in | Rubble-climb intro; Levies on the stairs |
| 2 | Great hall roofless; sky where rafters were | **Cinder Wraith** true intro, swooping between beam-hops |
| 3 | Armory racks stripped bare but for one child-sized helm | Brigands in a tight corridor; collapsing-floor trap |
| 4 | Spiral stair; arrow-slit light shafts full of ember-drift | Zigzag platform climb — the game's tallest built, spanning the full screen height — with Wraiths diving through the shafts; mid-climb checkpoint |
| 5 | **THE COLD HEARTH** — arena-sized dead hearth; the Warden's iron mantle in the ash; a kneeling-stone with a lantern cradle | Silent screen, no enemies. The lantern-cradle cards — the dual reveal, see THE TWIST — then **Warden's Coal**: Brand ignites; fireball tutorial on unlit braziers |
| 6 | Hearth-sigils painted inverted in soot — cultist graffiti | **Ember Cultist** intro lobbing fire from ledges; fireball is the counter-tool. First cultist kill toast: `They tithe to a nameless warmth.` |
| 7 | Throne room; the throne alone untouched and dustless | Trap gauntlet — swinging censers, spike pits — into an ambush wave |
| 8 | Broken east wall framing the war camp's glow — and on a distant rampart in that glow, one small ember-lit silhouette. Selwyn, seen once, far off | Long descent, mixed gauntlet; **KINDLED** transformation; checkpoint |

## ACT III — THE HUNGRY LIGHT *(unbuilt — full spec, free to iterate)*

> `His camp burned brighter than the kingdom.`
> `Nothing in it was warm.`

The act's job: stage the hero's self-blame at congregation scale, then take it away
from him for good. The camp is full of people who were told exactly what he was
told — *the fire found you wanting* — and he walks through what believing it makes
of a person.

Level-design reality check, baked in: every built level is one screen tall (17
tiles, no vertical camera); Acts I–II verticality is optional half-screen detours,
and there are only three lethal drops across all 16 built screens. Act III is where
the game earns its vertical — one true climb (engine-flagged below) and two lethal
fire hazards.

| # | Visual beat | Gameplay beat |
|---|---|---|
| 1 | **THE DOOR PALISADE** — a palisade built from the scorched house-doors of Caldermark homes | Bright firelight now hostile (the motif inversion begins); Cultists + Hounds together |
| 2 | **THE CAGE ROAD** — cage wagons, all empty, doors open — nothing kept, everything fed | Brigand pairs; fire trenches to leap — the trenches are lethal (fall risk 1 of the act) |
| 3 | **THE ASPIRANTS' WALL** — tithe-brazier ringed with offered gauntlets, hands and all; behind it a wall of soot-painted lanterns, each crossed out — one per convert; the crimson toy in the tithe-pile. And one cultist who does not attack: he kneels at the brazier, performing the hero's own lantern-lift with an empty gauntlet | Cultist nest wave (the kneeler excepted — he fights only if struck, and is worth no XP and breaks no chain; the game stays silent about him either way); heart-embers scarce from here on |
| 4 | **THE BANNER MOUND** — Caldermark's crimson banners piled for burning | **Hearthstone** (5th heart) hidden behind the mound; checkpoint |
| 5 | **THE FORGE STACK** — the horde forge built vertical: melt-channel below, scaffold and bellows above; kingdom coins go in, cleaver steel comes out. Ember-drift blows *upward* here — the one sanctioned break in the wind rule, because the heat column owns the sky | The climb: ~2.5 screens of genuine vertical; timed bellows-blasts as hazards, Wraiths diving through the smoke; the melt-channel below is lethal (fall risk 2). **Engine flag: this needs vertical camera scroll, which the engine does not have.** Fallback if the camera stays fixed: three chained single-screen tiers (5a/5b/5c) with a lethal drop guarding each ledge transition — same beat, no camera work |
| 6 | **THE FIELD OF VISORS** — ranked horde helms on posts, every visor dark. Only two visors in this world glow | Full-roster gauntlet |
| 7 | **THE AVENUE** — torches taller than houses; the hero's visor-glow vanishes against the blaze | No enemies. A dread walk. Final checkpoint. Silence is the beat |
| 8 | **THE PYRE** — arena: a bonfire of banners, Selwyn feeding it by hand | **BOSS**; **ABLAZE** reached during the fight |

**Act III checkpoint idle:** the familiar lantern-lift gains a half-second
hesitation before he performs it — fire feels different here. (The mechanical hinge
of the Act III inversion, taught through the animation the player has seen 15+
times. After the Cold Hearth he knows the darkness of his lantern was never an
answer — but the gesture is all he has, so he keeps making it, slower.)

## The boss — SELWYN THE WARM *(unbuilt — spec)*

> `SELWYN THE WARM`
> `He kept your fire. He keeps it still.`

The fight is the theme staged: a keeper against a hoarder — and the arena gives the
player a way to *win by tending*.

**The four braziers.** The arena holds four cold braziers. Any brazier the player
lights (fireball only — Embers spent on something other than damage) stays lit and
becomes tended ground. In phase 2, any floor-fire that reaches an *unlit* brazier
scorches its socket and locks it out — the window closes as Selwyn comes apart. In
phase 3, when the arena edges ignite, the ring around each tended brazier stays
cool: the only safe footing is the fires the player kept. The man the fire
supposedly refused keeps four hearths alive in the middle of a boss fight — the
redemption argued as mechanics, no text needed.

1. **The Warden** — slow, telegraphed cleaver arcs, a keeper's discipline guarding
   the coal in his chest; the man he was still holds the line. All four braziers
   are lightable.
2. **The Untended** — armor seams crack and vent (the same seam-glow the player has
   worn since Kindled); he ignites floor patches he then avoids feeding — the fire
   is escaping him; faster but sloppier. Floor-fires threaten unlit braziers. Pairs
   of Ash Imps skitter out of the bonfire (embers made flesh) — chain fodder, and
   the XP that carries the player over the ABLAZE line mid-fight.
3. **The Wildfire** — cleaver dropped half-melted; a walking bonfire doing
   Ash-Hound rushes as the arena edges ignite. **He brightens as his HP drops:**
   dying as pure spending. Tended braziers are the only cool ground.

**Gesture rhyme:** at each phase break, Selwyn cups the coal in his chest with both
hands — the keeper's carrying gesture curled shut into hoarding. The player will
see the same two hands open in the epilogue.

Phase transitions: 20f hitstop, white flash, palette shift hotter, 8px shake over
30f, arena torches flare. **Death beat — no text.** He gutters; the fire leaves him
standing, then the husk falls. Every light dies — the tended braziers gutter last,
one by one — except the King's Ember, glowing where he stood. Darkest screen in
the game.

## Epilogue (playable, silent) *(unbuilt — spec)*

At the dead great hearth, the King's Ember carried in both hands — open-palmed,
the keeper's gesture Selwyn curled shut. As the hero approaches, he instinctively
begins the lantern-lift he has performed at every checkpoint — then stops himself
mid-motion, lantern raised, awaiting input. That one held frame is the tell that
this moment is a decision. Press attack to kindle — or walk off-screen to refuse.
No prompt, no menu.

- **KINDLE:** he sets the Ember in the great hearth. As it takes, he lifts his
  lantern to it one last time — and this time it lights. The gesture the game has
  taught twenty times is finally answered; the stolen investiture completes, on his
  own terms, while his sprite already burns Ablaze.
  Cards: `The great hearth of Caldermark burned.` / `Tended, this time.` — a vow
  made by a man who now knows he was always fit for the watch.
- **REFUSE:** he sets the Ember in the ash and walks off-screen, lantern dark by
  choice for the first time. He ends the succession itself — lets the watch end,
  the one thing Selwyn could never do.
  Cards: `He left the ember to the cold.` / `No fire outlives its keeper twice.`

Either way the ending is his redemption: the choice is made free of the fault he
carried east. Unworthiness is not in the room; only judgment is.

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

Built (matches `index.html`):

| Moment | Line |
|---|---|
| Press start | `PRESS ENTER TO KEEP THE FLAME` |
| Crawl card 1 | `The King's Ember warmed all Caldermark.` / `Its Ember Warden was sworn to tend it.` |
| Crawl card 2 | `He stopped. It fed on him instead.` / `Then it fed on the kingdom.` |
| Crawl card 3 | `One knight lived, and blamed himself.` / `He marches east to take back the fire.` |
| Act I card | `ACT I — THE ASH HARVEST` · `The wind carried it east.` / `So he walked east.` |
| Act II card | `ACT II — THE COLD HEARTH` · `Every hearth in Caldermark was lit` / `from one fire. He knew where it lived.` |
| Coin (first) | `A dead man's coin. Carry it home.` |
| Heart ember | `An ember. It warms what it can.` |
| Hearthstone | `A hearthstone, still warm. Keep it.` / `+1 HEART OF WARMTH` |
| Warden's Coal | `A kept coal. Brand banks the heat.` / `C — HURL FIRE` |
| Fire-Steel | `A soldier's fire-steel. Struck true.` / `One strike in twenty will catch.` |
| Crit flash | `THE BLADE CATCHES` |
| Fireball empty | `BRAND RUNS COLD` |
| Checkpoint | `TENDED.` |
| Twist cards (II-5) | `The lantern fits the cradle.` / `It was never filled.` — then `A Warden fills his heir's lantern.` / `Selwyn never let his watch end.` |
| Level 1 | `SPARK. THE EMBER STIRS.` |
| Level 2 | `KINDLED. THE VISOR BRIGHTENS.` |
| Level 3 | `ABLAZE. HOW BRIGHTLY YOU BURN.` |
| Death | `One coal spent.` |
| Game over | `The lantern is empty.` / `The wind takes the rest.` |
| Act II end | `TO BE CONTINUED` / `ACT III — THE HUNGRY LIGHT` |
| Tally header | `HOW BRIGHTLY DID YOU BURN?` |

To build (Act III / boss / epilogue):

| Moment | Line |
|---|---|
| Act III card | `ACT III — THE HUNGRY LIGHT` · `His camp burned brighter than the kingdom.` / `Nothing in it was warm.` |
| Boss intro | `SELWYN THE WARM` / `He kept your fire. He keeps it still.` |
| Epilogue: kindle | `The great hearth of Caldermark burned.` / `Tended, this time.` |
| Epilogue: refuse | `He left the ember to the cold.` / `No fire outlives its keeper twice.` |

## Enemy lore (bestiary lines)

Full lines below; the build shows a compressed first-kill toast per kind
(e.g. `The kingdom's levy still musters.` · `The dogs stayed. The fire kept them.` ·
`Sellswords, paid in dead men's coin.`).

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
   The hero's idle there: lifts his lantern to the flame, lowers it, still dark —
   the rite, re-asked (see THE TWIST).
6. **Enemy visors and eye-slits are always dark** — pays off at III-6.
7. **Ember-drift always blows left-to-right** (the wind went east). One sanctioned
   exception: the Forge Stack (III-5), where the heat column blows it upward.
8. **Selwyn brightens as his HP drops;** after his death, the darkest palette in the
   game — the King's Ember the only warmth left.
9. **Paired lantern-brackets on every shrine, one always empty** — the twist,
   hiding in set dressing from screen 3.
10. **The lantern-lift is the game's signature gesture** — the hero at every
    checkpoint, the kneeling cultist at the tithe-brazier (III-3), Selwyn's
    closed-hand inversion at phase breaks, and the epilogue's answered lift.
    One motion, four meanings.
