---
type: build
patch: "0.4.0"
sources: [entangle-oracle-maxroll]
updated: 2026-05-21
tags: [druid, oracle, plant, caster, spell, endgame]
---

# Entangle Oracle

Druid / [[Oracle]] caster archetype. Plants vines via [[Entangle]] and detonates them with [[Thunderstorm]] for clear; [[Thrashing Vines]] covers single-target. Endgame pivots to a Life-cost spell engine using **Mind Over Matter** + **Eldritch Battery**, with Energy Shield converted to Mana acting as a second life bar.

First non-Ranger build documented in the wiki.

## Core gameplay loop

### Clear

1. Cast [[Entangle]] several times across the pack.
2. Cast [[Thunderstorm]] over the vines — the Accelerated Growth support causes the storm hits to detonate the vines into large nature explosions.
3. [[Thrashing Vines]] on rares / mini-bosses.

### Single target

1. Apply Temporal Chains before the boss aggros.
2. Cast [[Entangle]] multiple times into the boss.
3. Place [[Thunderstorm]] over them.
4. Spam [[Thrashing Vines]] (limit 1 by default; up to higher with Idol of Uldurn or Overabundance I).

## Ascendancy path

[[Oracle]] node order:

1. **The Unseen Path** — reveals special nodes.
2. **Entwined Realities** — allocate high-value notables without pathing to them.
3. **The Lesser Harm** — hit damage reduction; trade-off is reduced crit chance.
4. **Forced Outcome** — at "25% – 35%" investment, reroll crits for damage scaling.

## Key keystones

- **Wildsurge Incantation** — early campaign priority.
- **Mind Over Matter** — damage hits Mana before Life (endgame core).
- **Eldritch Battery** — converts Energy Shield to Mana (endgame core).

## Notables

Boundless Growth, Constricting, Cut to the Bone (Armour Break), Scarred Faith, Blackflame Covenant, Blood Transfusion (Life-casting transition), Sanguimantic Rituals (Arcane Surge conversion), Aspiring Genius (Arcane Surge source), Calculated Hunter, Give Up Your Essence. Undying Hate jewel (Tecrod variant) → Sacrifice of Blood.

## Defensive plan

- **Campaign**: Life-based caster. Stack Armour. Use "Armour applies to Elemental Damage" scaling. Cap 75% all-element resistance.
- **Endgame**: switch to Life-cost casting via **Atalui's Bloodletting** + Lifetap. This unlocks Mind Over Matter + Eldritch Battery — Energy Shield becomes Mana, which absorbs incoming damage before the Life pool.
- The Lesser Harm ascendancy provides an additional hit-damage reduction layer throughout.

## Sustain (endgame)

High spell Life-cost + Mana taking hits via MoM/EB makes sustain the critical stat:

- Mana Remnants, supported by Clarity I and Vitality I.
- Thunderstorm kept at low gem level for cost efficiency.
- Arcane Surge (sourced from Aspiring Genius) converted via Sanguimantic Rituals.
- Sacrifice of Blood scaling via Undying Hate (Tecrod variant).

## Offensive scaling priorities

1. +Physical Gem Levels, +Spell Gem Levels (primary).
2. %Spell Damage, %Spell Physical Damage.
3. Critical Strike Chance + Critical Damage Bonus.
4. Cast Speed.
5. Damage Gained as Lightning / Cold / Fire / Chaos.
6. Increased Duration (plant duration on the ground).
7. Increased Area of Effect (overlap + clear).

## Unique items

| Item | Phase | Role |
| --- | --- | --- |
| Bushwhack | Early campaign | Physical → Pin (3-second duration) |
| Idol of Uldurn | Early/mid | Amulet; +Limit for single-target skills |
| Atalui's Bloodletting | Endgame | Lineage support — Lifetap + Life-scaling damage |
| Atziri's Rule | Endgame | Staff with spell life leech; target "5% of Spell Damage Leeched as Life" corruption |
| Kurgal's Gaze | Endgame | Helmet; doubles values on Life regeneration nodes |
| Undying Hate (Tecrod variant) | Endgame | Jewel; Sacrifice of Blood scaling near Blackflame Covenant |
| Fast Metabolism | Endgame | Amulet instill |

## Leveling progression

| Level band | Skills | Notes |
| --- | --- | --- |
| 1–14 | Orb of Storms + Volcano + [[spark]] | Spirit gems: Arctic Armour, Mana Remnants (level 4) |
| 14–31 | [[Entangle]] + [[Thunderstorm]] | Grab Shock Conduction II support |
| 31+ | Full rotation incl. [[Thrashing Vines]] | Path toward Wildsurge Incantation |

Passive priority: spell damage + cast speed → plant nodes (Boundless Growth, Constricting) → Cut to the Bone (Armour Break) → Wildsurge Incantation.

## Endgame gear progression

- **Late campaign / early maps**: Staff with +Physical Gem Levels and +Spell Gem Levels. Cap resistances, attributes, Life, Armour, cast speed. Save divines for Atalui's Bloodletting.
- **Full endgame**: Atalui's Bloodletting + Atziri's Rule (corrupted variant) + Fast Metabolism amulet + Kurgal's Gaze + Undying Hate near Blackflame Covenant. Goal is to absorb the MoM/EB cost-flow without dipping Life.

## Weapon swap

The guide does not describe a weapon-swap setup. Single weapon (staff/wand) throughout.

## Cross-references with existing wiki

- Uses [[Spark]] in early campaign — same skill featured in [[Cold Spark Pathfinder]] but in a very different role here (level 1–14 only, replaced by Druid plant skills by level 14).

## Open questions

- Whether [[Entangle]], [[Thunderstorm]], [[Thrashing Vines]] are classified as **Primal Skills** per the 0.4 patch notes (they are plant-themed but not explicitly tagged in the source).
- Whether [[Oracle]] interacts with [[boss-anti-burst]] differently than other casters during pinnacle fights (no information in source).
- Whether 0.5.0 changes Druid skill costs in a way that breaks the Atalui's Bloodletting + MoM/EB chain.

## See also

- [[Oracle]]
- [[Cold Spark Pathfinder]] — for the [[Spark]] cross-reference
- [[patch-0.4.0]] — Druid class introduction
