---
type: build
patch: "0.4.0"
sources: [spiral-volley-deadeye-maxroll]
updated: 2026-05-21
tags: [spiral-volley, lightning, bow, ranger, deadeye, mapper]
---

# Spiral Volley Deadeye

A Ranger/[[Deadeye]] bow attack build. One-click 360° map clear with [[Spiral Volley]],
boss damage through stacked [[Lightning Rod]] + chained [[Lightning Arrow]]. Self-sustains
Frenzy Charges via the [[Resonance]] keystone loop.

> Newcomer-friendly summary: clear with Lightning Arrow until level 54, then unlock the
> "press one button, clear the screen" experience with Spiral Volley. Bosses die to a
> stack of Rods + spamming Lightning Arrow into them.

## Core engine: the [[Resonance]] loop

This is the only mechanic that makes the build work. Skip [[Resonance]] and the build
breaks.

1. [[Spiral Volley]] linked to **Armour Break III** + **Enduring Impact II**
2. Hits generate Endurance Charges (armour break + heavy stun)
3. [[Resonance]] converts Endurance → Frenzy
4. Frenzies empower the next Spiral Volley
5. Loop sustains as long as cast hits a few targets

Bow MUST have decent Physical Damage — only Physical breaks armour.

**Fallback:** Snipe + Perfected Endurance generates the first charge when out
(keep Snipe at level 3 for low mana cost).

## Phases

### Campaign (level 1-53, Lightning Arrow main)

- [[Lightning Arrow]] for clear, [[Lightning Rod]] for single target / damage check
- Spirit gems: Herald of Thunder (clear), Wind Dancer (evasion), Tame Beast with Haste Aura (damage + clear)
- Burst tools: Freezing Salvo (tanky enemies, hordes)

**Defense:** Life, Evasion, capped Resistances. Hybrid Evasion/ES bases as you find them.

**Deadeye order:** Gathering Winds → Endless Munitions → Point Blank → Called Shots

### Spiral Volley swap (level 54)

Allocate [[Resonance]] and swap clear to [[Spiral Volley]]. Required:

- [[Resonance]] keystone allocated
- Armour Break III + Enduring Impact II socketed in Spiral Volley
- **Respec Deadeye Point Blank → Far Shot** (don't forget this — big damage)
- Bow with Physical Damage

Cut a fresh level 1 [[Lightning Arrow]] gem at this point — its role is now purely
triggering [[Lightning Rod]] pulses, mana cost matters more than damage.

### Crit swap (when bow allows)

Trigger: bow has high damage + `+% to Critical Hit Chance` roll.

- Add Maligaro's Virtuosity (gloves) — sets Critical Damage Bonus to 250%
- Anoint Serpent's Egg with **Leaping Ambush** — carries crit chance
- Combined with Ambush, low tree investment for high crit chance
- Look for corruptions: higher Crit Damage multiplier, +1 maximum Frenzy Charges

### Endgame (ES, rare gear)

- Lean into Energy Shield: pure Evasion body armour + high-ES helmet (Subterfuge Mask passive)
- Ghost Dance: ES recovery on hit based on Evasion
- Headhunter — best mapping belt by a wide margin
- Optional: separate Bow+Quiver sets for clear vs single target
- Prism of Belief with `+levels to Spiral Volley`
- Megalomaniacs to save tree points

### Optional Pathfinder respec

Patch 0.4.0 buffed Running Assault to prevent knockdown while sprinting entirely.
Start as Deadeye → respec to [[Pathfinder]] once gear is good enough to not need
Deadeye's damage. Gives risk-free +120% Movement Speed sprint.

## Rotations

### Clear (post-54)

1. Hit anything → gain first charge (via Snipe if out)
2. Spiral Volley into a mob — regenerates Frenzies
3. Keep going
4. When Frenzies run out → back to step 1

Once gear is strong enough to Armour Break/Heavy Stun white mobs without Frenzies,
the build no longer cares about target count per cast.

### Basic single target

1. Stack ~20 [[Lightning Rod]] casts on boss (replaces decaying rods, sustains the 10 cap)
2. Spam [[Lightning Arrow]] into them

### Advanced single target

1. **Before** boss spawns: stack 20 Rods at spawn location
2. Single Tornado Shot at the boss spawn point (level 41+)
3. Barrage once
4. Spam [[Lightning Arrow]]

Tornado Shot absorbs and re-emits arrows, multiplying Rod activations.

## Weapon swap setup

- **Weapon Set 1**: [[Lightning Arrow]] + [[Lightning Rod]]
- **Weapon Set 2**: [[Spiral Volley]]
- Order matters for Rigwald's Ferocity
- Persistent buffs on both sets
- Clone bow + quiver to second set via the empty-hand right-click trick on the (I) button

## Stat priorities

**Offensive:**
- Bow (everything — high Physical + Elemental Damage)
- Bow Attacks Fire an Additional Arrow (Lightning Rod only — Spiral Volley doesn't benefit)
- `+# to Level of all (Projectile) Gems`
- Gain % Damage as extra Fire/Cold/Lightning
- Flat Fire/Cold/Lightning/Physical Damage to Attacks
- Crit Chance, Attack Speed, Projectile Speed
- Attributes (Int/Dex/Str — convert via Passive Tree respec)

**Defensive:**
- Capped resistances (incl. Chaos)
- Maximum Life
- Evasion Rating (main avoidance)
- Deflection
- Endgame: Energy Shield buffer

**Mana sustain:** Sapphire Jewel with `Recover 2% of Mana on Kill` + `Gain # Mana per Enemy Killed`
on bow or quiver.

## Key uniques (mentioned, not yet wiki pages)

- **Serpent's Egg** — triples charge generation, "buy ASAP" priority
- **Cadiro's Gambit** — 29-arrow Spiral Volley guarantees every effect rolls
- **Maligaro's Virtuosity** — crit swap enabler (shared with [[Cold Spark Pathfinder]])
- **Hyrri's Ire** — budget alternative to rare chest
- **Headhunter** — endgame mapping belt
- **Rigwald's Ferocity** — interacts with weapon-swap order
- **Prism of Belief** — `+levels to Spiral Volley`

## Why this build for new players

- Defined progression checkpoint at level 54 — clear "before/after" of the build
- Once Resonance loop is set up, gameplay is genuinely one-button for mapping
- Bow attack is easier to position than spells (longer range, less commitment)
- Optional Pathfinder respec gives an upgrade path without rerolling

## Pitfalls

- Forgetting Point Blank → Far Shot at 54 (big damage loss)
- Bow without Physical Damage → no armour break → no Frenzies → no damage
- Trying Spiral Volley before allocating [[Resonance]] (build does not work)
- Cast on Critical (last gem!) — not used in this build; that's a [[Cold Spark Pathfinder]] convention
