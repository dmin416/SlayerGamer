# Gacha Rules

Live system reference for D. Source pattern: `Slayer Gamer Source\The_Slayer_Gamer.txt` (Iris) plus the design tables below.  
Catalog of Tavish’s spent pulls: `Original_Story_Gacha_Pulls.md`.  
Kill / box loot (not snaps): `loot-rules.md`.

**Flow:** *kill → body + on-person (always) → independent box roll (Luck/10000) + independent token roll (Luck/200) → on token hit: family → rarity (if any) → bank unspent → (on spend) snap tables.*

Gacha is **not** the corpse. Loot boxes and skill books are separate (`loot-rules.md`). No forced kill tokens or boxes.

---

## 0. Effective Luck

Printed %-Luck items use:

**Effective Luck = floor( Base Luck × (1 + sum of item percents) )**

Always **round down** after the multiply. Fractional Effective Luck is never used mid-roll.

Examples: Daisy +75% → ×1.75. Fry’s clover +77% → ×1.77. Both owned → ×(1 + 0.75 + 0.77) = ×2.52 (**additive percents**, not multiply-the-multipliers). Luck 20 × 2.52 = 50.4 → **Effective Luck 50**.

Use **Effective Luck** everywhere Luck appears: kill drop, box drop, upgrade chain, and snap rarity roll.

| Item | Bonus | Notes |
| --- | --- | --- |
| Daisy’s Rabbit Foot (Tavish) | **+75% Luck** | Mythic gacha; not D’s |
| **Fry’s Seven-Leaf Clover** (D remap, if drawn) | **+77% Luck** | Seven-leaf charm; percent, not flat +77 |

**D has not spent opening gacha;** do not apply the clover until owned and held/equipped as play says.

### Luck 100 — Double or Nothing (D)

Replaces original **Lucky penny** for D. Unlocks at Effective Luck **≥ 100**.

If a **Luck-gated chance roll fails**, he may immediately make **one** reroll of that same check and keep the second result. Examples: kill token drop (Luck/200), kill box drop (Luck/10000), box rarity-upgrade gates that use Luck/d20. Family/rarity tables after a token already dropped are not “fail a Luck chance” unless a gate is Luck-thresholded.

- First roll success → no second roll, no double award.
- First fail → optional second roll; second fail = nothing.
- One reroll per check. Not a free second token/box on top of a hit.

---

## 1. How tokens are gained

### Kill drop (chance)

Tokens stay **Luck/200** (common). Boxes are **Luck/10000** (sparse at high Luck). See `loot-rules.md`.

**Token base = Effective Luck / 200.** Roll **d1000 ≤ min(1000, Effective Luck × 5)** on a normal kill. One success = **one token**. No guarantees.

| Enemy | Multiplier | Token thr (d1000) | Box thr (d10000) |
| --- | ---: | ---: | ---: |
| Normal | ×1 | min(1000, Luck × 5) | Luck |
| **Elite** | **×3** | min(1000, Luck × 15) | min(10000, Luck × 3) |
| **Boss** | **×10** | min(1000, Luck × 50) | min(10000, Luck × 10) |

Elite / boss tags follow the fight. Rabbit ID: White/Brown foragers = normal; **Greater** = elite; **Alpha** = boss.

Independent of the box roll. Clear-package and opened-box ledger tokens stay as printed; kill-drop tokens are **added** from audited kills.

**Opened-box priority:** if that kill’s opened box already printed a token, ledger wins for that kill’s token line (no second free kill-token unless the ledger says both). Unopened boxes do not block the token roll.

### Kill-drop family (after a token hits)

Roll **d1000**. **Companion is not on this table** (quest / world boxes only).

| d1000 | Family | Rate | Has rarity? |
| --- | --- | ---: | --- |
| 001–750 | Standard gacha | 75% | yes |
| 751–850 | Skill | 10% | yes |
| 851–900 | Challenge | 5% | **no** (flat Challenge token) |
| 901–940 | Perk | 4% | yes |
| 941–970 | Class | 3% | yes |
| 971–990 | World | 2% | **no** (flat World token) |
| 991–000 | Race | 1% | yes |

### Kill-drop rarity (families that have it)

**No upgrade chain** on kill tokens. Rarity is this roll only.

**Standard gacha**

| Rarity | % | d1000 within family |
| --- | ---: | --- |
| Common | 80 | 001–800 |
| Rare | 12 | 801–920 |
| Epic | 5 | 921–970 |
| Legendary | 2 | 971–990 |
| Mythic | 0.8 | 991–998 |
| God-tier | 0.2 | 999–000 |

**Skill / Perk**

| Rarity | % | d1000 within family |
| --- | ---: | --- |
| Common | 70 | 001–700 |
| Rare | 18 | 701–880 |
| Epic | 8 | 881–960 |
| Legendary | 3 | 961–990 |
| Mythic | 0.8 | 991–998 |
| God-tier | 0.2 | 999–000 |

**Class**

| Rarity | % | d1000 within family |
| --- | ---: | --- |
| Common | 55 | 001–550 |
| Rare | 25 | 551–800 |
| Epic | 12 | 801–920 |
| Legendary | 5 | 921–970 |
| Mythic | 2 | 971–990 |
| God-tier | 1 | 991–000 |

**Race**

| Rarity | % | d1000 within family |
| --- | ---: | --- |
| Common | 40 | 001–400 |
| Rare | 30 | 401–700 |
| Epic | 18 | 701–880 |
| Legendary | 8 | 881–960 |
| Mythic | 3 | 961–990 |
| God-tier | 1 | 991–000 |

Challenge / World: skip rarity. Bank as **Challenge token** or **World token**.

### Upgrade chain (non-kill tokens only)

For printed clear/quest packages or other sources that still climb. **Not** after kill-drop family/rarity rolls.

| Trying to reach | Method |
| --- | --- |
| **Rare** | d1000 ≤ Effective Luck |
| **Epic** and each tier above | d20 need **20**, **+1 per 50** Effective Luck |

### Other sources

| Source | What happens |
| --- | --- |
| Clear / grind **Loot Gained** dumps | Batched tokens as printed (e.g. first ID **5 Common + 1 Epic**). Separate from kill Luck/200. |
| Quest / challenge reward lines | Fixed packages as printed. |
| Kill-loot / quest boxes | Contents per ledger. **Companion tokens** only from quest / world boxes, not kill-token RNG. |
| **Gacha Gambler** perk | **1 free Common draw per week** (free snap, not a banked token). |

**D’s live unspent counts:** Inventory checkpoints. Do not invent spends.

---

## 2. Token types (what a snap can roll)

| Token | Draws from | Notes |
| --- | --- | --- |
| **Common** | Poor through God-tier | Bulk of tokens. Junk-heavy. |
| **Rare** | Rare and up (Poor/Common/Uncommon out) | Narrower pool. |
| **Epic** | Epic and up | Often a related **batch** (see Step 3). |
| **Legendary** | Legendary and up | Between Epic and Mythic. |
| **Mythic** | **Mythic and up** | Story-shaping. High God chance by design. |
| **God-tier** | **God-tier only** | Direct God token. |
| **Perk Token** | Perks only | Skips category swim. |
| **Skill Token** | Skills / skill books only | Skips category swim. |
| **Class / Race / World Token** | Fixed meta category | Receive ≠ activate. Class token / Class scroll opens a category menu; must meet prereqs before leveling. Prestige stays one-at-a-time; multi-standard after Lv40; production is the Lv5 craft slot (`Timeline.md`). Challenge/World kill drops are flat (no rarity). |
| **Companion Token** | Named companion | **Not** from kill-token RNG; quest / world boxes. |
| **Challenge Token** | Challenge select | Flat; no rarity on kill drops. |

Iris (original): Common can hit any category; Rare excludes common-tier results. Tables below fill unprinted bands.

---

## 3. Snap procedure

Two independent rolls on a standard gacha token: **rarity** (d100 by token type), then **category** (d20). Then name one concrete result. Do not upgrade rarity after the roll.

Perk / Skill / Class / Race / World / Challenge / Companion tokens skip the category swim and resolve in their fixed pool (rarity table still applies when the token has rarity).

### Step 1: Rarity (d100)

Each column sums to 100%.

| Result | Common | Rare | Epic | Legendary | Mythic | God-tier |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| Poor | 20% (01-20) | — | — | — | — | — |
| Common | 35% (21-55) | — | — | — | — | — |
| Uncommon | 15% (56-70) | — | — | — | — | — |
| Rare | 15% (71-85) | 55% (01-55) | — | — | — | — |
| Epic | 9% (86-94) | 30% (56-85) | 60% (01-60) | — | — | — |
| Legendary | 4% (95-98) | 11% (86-96) | 30% (61-90) | 45% (01-45) | — | — |
| Mythic | 1% (99) | 3% (97-99) | 9% (91-99) | 40% (46-85) | 70% (01-70) | — |
| God-tier | 1% (00) | 1% (00) | 1% (00) | 15% (86-00) | 30% (71-00) | **100% (01-00)** |

**Floor (at least this rarity, single d100 before Luck):**

| Token | ≥ Rare | ≥ Epic | ≥ Legendary | ≥ Mythic | ≥ God-tier |
| --- | ---: | ---: | ---: | ---: | ---: |
| Common | 30% | 15% | 6% | 2% | 1% |
| Rare | 100% | 45% | 15% | 4% | 1% |
| Epic | 100% | 100% | 40% | 10% | 1% |
| Legendary | 100% | 100% | 100% | 55% | 15% |
| Mythic | 100% | 100% | 100% | 100% | 30% |
| God-tier | 100% | 100% | 100% | 100% | 100% |

**Luck on the rarity roll (Common, Rare and Epic tokens only):** roll **1 extra d100 per 100 Effective Luck** (max 3 extra) and **keep the highest**. 00 counts as 100. Legendary, Mythic and God-tier tokens roll one d100.

### Step 2: Category (d20)

| d20 | Category | Likelihood |
| --- | --- | ---: |
| 1-4 | Junk / Comedy | 20% |
| 5-8 | Weapon | 20% |
| 9-10 | Armor / Gear | 10% |
| 11 | Consumable | 5% |
| 12 | Skill Book / Scroll | 5% |
| 13 | Perk | 5% |
| 14 | Material | 5% |
| 15 | Tech / Blueprint | 5% |
| 16 | Vehicle / Mount | 5% |
| 17 | **Pet / Familiar** | 5% |
| 18 | Property / Base | 5% |
| 19 | Currency / Wealth | 5% |
| 20 | **Meta Token** (Class / Race / World / **Companion**) | 5% |

**17 vs 20:** Pet/Familiar = animal, mascot, low-story pet. Meta Companion = named story-level ally token (Ty-class, Harley-class). Mounts with no story role stay Vehicle (16). Companion via this snap path is still possible from a **standard gacha** category-20 hit; dedicated Companion **tokens** stay quest/world-box only.

**Bad combo:** Poor or Common rarity in Vehicle, Property, Pet/Familiar, Meta, Perk or Currency resolves as a **scrap / toy / fragment / stray** of that type (never a full vehicle, deed, named companion or class).

**Meta rarity:** Common Meta → basic / joke-tier option. Higher token or rolled rarity → stronger pool (Mythic Class ≠ Common Class).

**Perk / Skill tokens:** category fixed. Use the snap rarity table for the token’s printed rarity.

### Step 3: Name the result

One concrete item matching rarity + category.

**Epic token batch:** on an **Epic token** that rolls Epic, name **1d8+4** related items (5–12). Any higher roll gives **1** item. One category roll covers the whole batch.

Junk/Comedy stays junk even on a high token unless that token type already excluded Poor/Common.

---

## 4. Worked example

Kill a **Common** forager (normal). Effective Luck **75**.

1. **Box:** d10000 ≤ 75? separate. Assume miss.
2. **Token:** d1000 ≤ 375 (75×5)? roll 210 → hit.
3. **Family:** d1000 → 612 → Standard gacha.
4. **Rarity:** d1000 → 845 → **Rare** standard gacha. Bank it. No upgrade chain.
5. Later **spend** the Rare token: snap rarity d100 + category d20 + name.

---

## 5. Restrictions

- Receipt ≠ use. Do not auto-apply mid-prose without a spent token.
- Meta tokens from gacha are **received**, not auto-activated.
- Kill-token Companion family is **off**. Companion tokens come from quest / world boxes.
- Keep snaps distinct from quest clear packages and kill-loot box contents (`loot-rules.md`).
- D’s bag lists **token counts** until he spends. Do not paste Tavish pull results into live Inventory.
