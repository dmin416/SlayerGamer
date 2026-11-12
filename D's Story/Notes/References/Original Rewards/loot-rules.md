# Loot Rules

Live system reference for D. Source pattern: `Slayer Gamer Source\The_Slayer_Gamer.txt`.  
Token snaps: `gacha-rules.md`. Tavish spent-pull catalog: `Original_Story_Gacha_Pulls.md`.  
RE2 kill-box ledger: `..\World Specific\03 Resident Evil 2\RE2_Loot_Box_Openings.md`.

---

## 1. Rarity tiers

Poor → Common → Uncommon → Rare → Epic → Legendary → Mythic → God-tier

**Iconic** is an extra tag for an item tied to a famous owner (e.g. a named character’s personal gun). Gacha copies are usually “similar model,” not the iconic original (Iris).

---

## 2. What a kill grants

### Always (body + person)

On a kill, expect:

1. **The body** (or usable remains): meat, hide, horn, bone, organs, carcass parts, wreckage, etc., as the creature/world allows. Chef worlds harvest this.
2. **What was on its person:** worn gear, carried weapons, pockets, packs, ammo, cash, keys, junk it was holding. Animals with no kit still give body/harvest; armed foes give kit + body.

Luck can still color **quality / quantity** of that haul (better cuts, denser pockets), especially on elites/bosses. Do not skip the body/person baseline and replace it with a mystery roll.

### Separate rolls (not automatic with the body)

No forced tokens. No forced boxes. No forced skills. Independent rolls per kill (can hit any, all, or none).

**Double or Nothing** (Luck ≥ 100): on a **failed** Luck-gated drop/upgrade roll, one immediate reroll of that check (`gacha-rules.md`). Creation LCK 77 does not have it yet.

| Roll | Rule |
| --- | --- |
| **Loot box** | **Luck / 10000** (d10000 ≤ thr). Elite **×3**, boss **×10** (cap 10000). Rarer than tokens on purpose. See §3. |
| **Token** | **Luck / 200** (d1000 ≤ Luck×5). Elite **×3**, boss **×10**. Then family + rarity per `gacha-rules.md`. |
| **Kill skill** | **Half the token threshold** (d1000 ≤ floor(token thr ÷ 2), after the token cap). Same elite ×3 / boss ×10. A hit gives **one skill taken from the creature killed** (a Licker gives a Licker-style skill). Rarity uses the Skill row of the kill-drop rarity table (`gacha-rules.md`). Skill tokens are separate (the token roll). |
| **Other skill sources** | Dungeon scatter, quest, or practice unlock. A corpse never grants a skill book. |
| **Quest / clear packages** | Separate. Printed at objectives, not per body. |

Biomass / DNA: only after a slime/symbiote is **bonded** in play (see §4).

### On-person / harvest flavors

| Flavor | Typical contents |
| --- | --- |
| Body / harvest | Meat, organs, hide, horn, bone, wreck parts (Chef / craft worlds) |
| Worn / carried | Guns, tools, armor, clothes, ammo |
| Pockets / pouch | Cash, junk, herbs, food, potions |
| Key / story | Keys, files, plot items only if it was carrying them |

Trash enemies lean Poor/Common kit. Elites/bosses lean richer on-person and denser harvest. Do not invent boss kit that breaks one-world continuity.

### Original examples (goblin ID)

- First kill: loin cloth + spear (on person) + cooked squirrel / cash texture; **no** gacha.
- Scout fight: cloths, spears, club, Rare cleaver on persons; **no** per-kill gacha.
- Area clear dump: body/kit stacks **plus** separate batched gacha (5 Common + 1 Epic).
- Grind dumps: kit stacks **plus** separate batched Common gacha.

For D’s rabbit remap: weapons → **body harvest** (horns, bones, feet, meat). Rare cleaver → Rare Pan (found in the clear, not a rabbit “sword”). Kill RNG tokens/boxes stay separate from printed clear packages.

---

## 3. Kill-loot boxes

Separate from body/person and from kill tokens. **No elite/boss guarantee.** Boxes are **held unopened** until opened in play / ledger.

### Drop chance (default worlds)

**Base = Effective Luck / 10000** (one more zero than the old /1000 feel, so high Luck does not rain boxes).

| Kill tag | Threshold (d10000) |
| --- | --- |
| Normal | Effective Luck |
| Elite | min(10000, Effective Luck × 3) |
| Boss | min(10000, Effective Luck × 10) |

Success = **one** box at that fight’s **floor** rarity, then the upgrade chain below.

**Horned Rabbit floors (when a box drops):** forager / Greater → **Common**; Alpha → **Epic**.

### Box rarity upgrade (after the floor exists)

| Trying to reach | Method |
| --- | --- |
| **Rare** (from Common / Uncommon floor) | d1000 ≤ Effective Luck |
| **Epic** and each tier above | d20 need **20**, **+1 per 50** Effective Luck |

A failed climb leaves the floor box.

### How much a box contains (D campaign count)

**Slots = rarity rank × 3 + 1**, with **Common = rank 1**.

| Box rarity | Rank | Slots |
| --- | ---: | ---: |
| Common | 1 | **4** |
| Uncommon | 2 | **7** |
| Rare | 3 | **10** |
| Epic | 4 | **13** |
| Legendary | 5 | **16** |
| Mythic | 6 | **19** |
| God-tier | 7 | **22** |

One slot = one named line (item, stack, or token) **unless slots are combined** (below). Mixed rarities inside a box are fine. **Kill boxes have a random origin:** contents can come from any world, game or franchise and do not follow the kill or the world it happened in. Skill books, perks, tokens and Funko-style figures can all appear (original almost always had a Funko in world crates). **Quest boxes are the opposite:** themed from the world and quest they came from.

### Combining slots

When opening a box, slots may be **spent together** instead of resolved one-for-one.

| Combine | Result |
| --- | --- |
| **2 slots** | One line at **+1 rarity rank** over the box floor, **or** same rank but **more specific** (named pick / tighter theme) |
| **3 slots** | One line at **+2 ranks**, **or** +1 rank and specific |
| **4 slots** | One line at **+3 ranks**, **or** +2 ranks and specific |
| Each extra slot beyond 4 | **+1 rank** further, or more specificity at the current rank (no free infinite climb past God-tier) |

Rules of thumb:

- Combined line **replaces** the spent slots (a 10-slot Rare opened as 3+3+4 → three lines, not ten).
- You can mix: some singles, some combines, in one open.
- **Specific** means choosing a clearer category or named target (e.g. “a plant skill book,” “a cooking perk,” “carrot-line seeds”) within what that rank can bear. It is not a free God-tier wish from Common slots.
- Token lines can be combined the same way (e.g. 2 slots → Rare standard token instead of Common), still **no Companion** from kill-box combines unless a quest/world box says so.
- RE2’s already-accepted opens are not rewritten. Future opens (and any agreed rabbit redo) may use combines.

**Original story background:** Iris never printed a slot formula; prose opens ranged from 1 item to jumble/hauls. D’s count + combine rules above are the live campaign layer. RE2 ledger stays as accepted history.

Companion tokens still prefer quest/world boxes. Unopened boxes do not block Luck/200 kill-token rolls.

Ch1 warren box audit at LCK 77 under /10000: **0** boxes (`Inventory - 01`).

---

## 4. Symbiote biomass / DNA (post-bond only)

Applies only after a slime/symbiote is bonded in play. Body still exists as harvest/loot; biomass is an extra track.

1. **Biomass** – organic matter absorbed; fuels morphs / regen / evolutions (replaces Soul Well style spend for that track).
   - After **Organic Metallization** (if gained): metal, robots, machines count as Biomass.
   - After Swamp Thing-style upgrade (if gained): plant matter at full value.
2. **DNA sample** – species integration bar 0–100%.
   - Touch samples; kill adds a large chunk; consuming the body adds more + Biomass.
   - **25%** minor passive · **50%** partial morph · **100%** signature trait + full morph option.
   - Non-biological (robots, golems, undead, spirits): **no DNA**; normal loot / tech still apply.

Trait examples once bonded: Slime (Liquid Body, Absorption); Licker (wall-crawl, hearing); Tyrant-class (strength, durability within story limits); Plant 43-line (growth, toxin, rooting).

---

## 5. Restrictions

- Body + on-person are the default kill result. Tokens and boxes are chance-only. No world or challenge grants a box per kill.
- Companion tokens are **not** on the kill-token table; leave them to quest / world boxes.
- A skill book is never assumed from the corpse. A kill skill is its own roll (see §2).
- Tokens carry no source. A token is a token wherever it dropped; its kill or world has no effect on what it snaps into.
- Symbiote rows stay off until bond exists on page.
- Quest clear packages are tracked on Inventory / `gacha-rules.md`.
- Tribute / Eternal Cycle is a separate kill track (Status), not a loot-box open.
- No second inventing of RE2 (or other) box contents outside the accepted ledger.
