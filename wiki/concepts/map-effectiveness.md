---
type: concept
patch: "0.4.0"
sources: [patch-0.4.0]
updated: 2026-05-21
tags: [endgame, mapping]
---

# Map Effectiveness

Map Effectiveness replaced pack size scaling on maps in patch 0.4.0.

## How it works

Effectiveness scales with [[waystone]] tier. When applied to non-unique monsters in a map, it grants:
- Increased monster life
- Increased experience granted
- Increased quantity of items dropped

Effectiveness does **not** change the number of monsters in the map. It makes each individual monster harder and more rewarding.

## Sources of effectiveness

- Tier-based base scaling on [[waystone]]s.
- **Challenger's** tablet modifier — 7–11% increased Effectiveness of Monsters in Maps (added in 0.4.0). See [[tablet-crafting]].
- **Xesht's Madness** Atlas Notable — Rare Breach Monsters have 50% increased Effectiveness (reworked in 0.4.0).

## Why this matters

Pre-0.4 builds optimized for pack size at high tiers to inflate density. With effectiveness replacing tier-scaled pack size, individual monster value goes up but density does not automatically scale with tier.

Practical implications:
- Single-target damage matters more relative to clear speed at high tiers.
- Survivability per encounter matters more than fast-rolling through low-HP packs.
- Pack-size tablet mods (Breeding, Teeming, Brimming) are the primary way to boost density now.

## Open questions

- Exact effectiveness % per tier is not documented in the patch notes.
- How effectiveness stacks multiplicatively with pack-size mods at very high tiers needs empirical testing.
- Does effectiveness influence boss difficulty or only non-unique monsters? Patch notes specify non-unique only.

## See also

- [[tablet-crafting]]
- [[endgame-0.4.0]]
- [[patch-0.4.0]]
