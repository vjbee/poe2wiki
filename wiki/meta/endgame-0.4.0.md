---
type: meta
patch: "0.4.0"
sources: [patch-0.4.0]
updated: 2026-05-21
tags: [endgame, baseline, atlas, tablets, bosses]
---

# Endgame State — Patch 0.4.0 Baseline

Snapshot of the PoE 2 endgame as it stood in patch 0.4.0 (Dec 2025–May 2026). Maintained as the comparison baseline for [[patch-0.5.0]] "Return of the Ancients", which is announced as a full endgame overhaul (release: May 29, 2026).

When 0.5 is ingested, this page should not be edited. A new `meta/endgame-0.5.0.md` page will be created, and a follow-up `meta/endgame-diff-0.4-to-0.5.md` will track the actual changes.

## Atlas content layers (0.4)

Active layers on the [[atlas-passive-tree]] in 0.4:
- [[breach]]
- [[delirium]]
- [[ritual]]
- [[expedition]]
- [[abyss]] (newly promoted from league mechanic to core in 0.4.0)
- Trial of the Sekhemas
- [[fate-of-the-vaal-league]] mechanic (current league overlay)

## Map scaling

Pack size scaling on maps was removed in 0.4.0. Replaced with [[map-effectiveness]], which scales monster life, experience granted, and item drop quantity per non-unique monster as waystone tier increases. Pack count itself is no longer tied to tier.

## Tablet system (0.4 state)

[[tablet-crafting]] cap is 4 modifiers per tablet.
- Slots 1–2: craftable immediately.
- Slots 3–4: gated behind a current-league [[arbiter-of-ash]] kill.
- All modifiers from "Precursor Tablet" can roll on any basetype.

### Modifiers added in 0.4.0

| Modifier | Effect | Notes |
|---|---|---|
| Challenger's | 7–11% increased Effectiveness of Monsters | Pairs with the new effectiveness scaling |
| of Contest | Unique Monsters have 1 additional Rare Modifier | |
| of Undertaking | Map has 1–2 additional random Modifiers | Re-enabled |

### Modifiers disabled in 0.4.0

| Modifier | Previous effect |
|---|---|
| Plundering | 4–10% increased Quantity of Items in Map |
| of the Pursuit | Delirium kill reward progress bonus |
| of Envy | Delirium encounter extra reward chance |

### Modifier ranges widened (selected)

Most existing tablet modifiers had their lower bound raised toward the high end. Examples:
- Collector's: 10–30% → 18–30% rarity
- Breeding: 4–10% → 6–10% pack size
- Teeming: 25–70% → 50–70% magic monsters
- Brimming: 15–40% → 25–40% rare monsters
- Bountiful: 15–40% → 25–40% gold
- Elevated: 5–20% → 10–20% experience
- of the Nemesis: 30–80% → 50–80% extra rare modifier chance
- of Shrines / Strongboxes / Essences / Spirits: 50–100% → 70–100% chance

See [[patch-0.4.0]] for the full diff list.

## Waystone changes (0.4)

- "Of Fleeting" restricted to T11+ waystones; value 10–15% (previously 21–25%).
- Waystones can no longer be instilled with [[liquid-emotions]].

## Pinnacle boss — Arbiter of Ash

[[arbiter-of-ash]] is the pinnacle endgame boss and the gating mechanism for advanced tablet crafting in 0.4.

Changes in 0.4.0:
- No longer drops a rare corrupted Tablet.
- Phase transition triggers at a lower life threshold.
- Heals to full during the phase transition.

## Boss damage mechanic

[[boss-anti-burst]] applies to bosses with emerge or aggro animations:
- Damage reduction starts at full effect when the boss emerges or becomes aggro.
- Tapers to zero over a fixed duration.
- Boss movement away from spawn accelerates the falloff.
- Stationary or near-stationary bosses have a shorter total reduction window.

Effect on builds: instant-kill strategies on emerge are no longer viable. Sustained DPS is required to clear the anti-burst window before the boss can be dropped.

## Atlas Notable changes (0.4)

### Waystone
- **The High Road**: reworked. Now grants 10% chance for Waystones found in maps to be Rare and Corrupted (previously +1 tier chance).

### Breach
- **Xesht's Madness**: no longer grants Soul Eater to rare Breach monsters. Now grants Onslaught and 50% increased Effectiveness to rare Breach monsters.

### Delirium
- **Get out of my head!** and **The mirrors... the mirrors!**: swapped positions on the tree.
- **Get out of my head!**: reworked around magic monster delirium modifiers (extra mod chance + rarity bonus on multi-mod kills).
- **Isn't it tempting?**: reworked. Map boss steals delirium currency drops, which has a chance to duplicate on boss kill.
- **It's not real, it's not real!**: reworked. Rare monsters always manifest delirium demons; bonuses to quantity and xp on those kills.

### Removed
- **Prayer for Wealth**: removed entirely. Greed Shrines no longer exist in the game.

## Delirium system (0.4)

- Reward bar indicator removed.
- Delirium monsters drop [[liquid-emotions]] directly.
- Delirium bosses guarantee a drop, with a chance of higher-tier emotions.
- Simulacrum boss waves also guarantee a drop.
- Delirium fog visuals improved with a clarity radius around the player.

## Other endgame changes

- [[abyss]] is now a core mechanic with its own [[atlas-passive-tree]] section.
- Idols of Estazunti no longer required for [[vaal-vault-maps]]. Existing items deleted.
- Vaults of Kamasa unique map chests no longer affected by party bonuses.
- Camera zoom-out on tower map completion removed.
- Activating all checkpoints + completing the map now reveals all minimap icons.
- Breach, Ritual, Delirium, Expedition removed from the Map Legend (no longer have icons shown on Atlas).

## Expected 0.5 impact

[[patch-0.5.0]] "Return of the Ancients" has been announced as a full endgame overhaul. Based on GGG communications and trailers, likely changes include:
- Mapping system restructure (death penalty changes, reward loop changes).
- Atlas Tree adjustments (potentially major).
- New endgame quest content and Atlas Fortress zone.
- Runes of Aldur league mechanic layered on top.
- Two new Ascendancies.

The 0.4 state above should be treated as ephemeral. After 0.5 is ingested, every section here should be revisited point-by-point.
