---
type: build
patch: "0.4.0"
sources: [cold-spark-pathfinder-maxroll]
updated: 2026-05-21
tags: [spark, cold, ranger, pathfinder, caster, projectile]
---

# Cold Spark Pathfinder

A Ranger-class spellcaster build using [[Spark]] converted to cold damage, scaled by
[[Cold-Infusion]] generation and the mobility/efficiency of the [[Pathfinder]] ascendancy.

> Newcomer-friendly summary: cast [[Frost Bomb]] to generate Cold-Infusions, then spam
> [[Spark]] to clear screens. Move freely while casting. Don't get stunned while sprinting.
> End-game adds Cast on Critical Comet for boss damage.

## Core loop

**Clear:**
1. Cast [[Frost Bomb]] on cooldown — generates [[Cold-Infusion]]
2. Cast [[Spark]] while infused

**Single target:**
1. Pre-stack [[Frost Bomb]] for infusions
2. Weapon swap to The Whispering Ice → Icestorm to apply Elemental Exposure
3. Cast Elemental Weakness (or Despair late)
4. Spam [[Spark]] until infusions run out, repeat

## Phases

### Campaign (Life / Evasion)

- Use [[Spark]] from level 1 with Projectile Acceleration III, Prolonged Duration II,
  and Fork (or Pierce II)
- Add [[Frost Bomb]] with Short Fuse I + Overabundance I (later Spell Cascade)
- Spirit gem: Arctic Armour (then Siphon Elements + Mana Remnants)
- Orb of Storms with Overabundance I + Unleash for layered damage

**Ascendancy with leveling gear:** Relentless Pursuit → Running Assault
**Ascendancy without:** Path Seeker → Traveller's Wisdom

**Passive priorities:** projectile damage, spell damage, elemental damage. Key nodes:
Thin Ice, Heavy Frost (ignores resistances), Kite Runner, Effervescent, Turn the
Clock Forward, Preservation. Allocate `Secrets of the Orb` for the 3rd Cold-Infusion.

**Campaign-friendly uniques (not required):**
- Painter's Servant (gloves) — converts spark to all three elements
- Crown of the Victor — +1 to all skills, life/mana on kill
- Enfolding Dawn + Threaded Light — early spell damage
- Grip of Kulemak — cast speed + damage gain (light radius downside)
- Astramentis — pairs with Traveller's Wisdom

### Maps (transition to Chaos Inoculation)

- Cap resistances, then prioritize Energy Shield from body armour
- Pick up Critical Hit Chance / Critical Hit Chance for Spells
- Wand with `+Spell Gem Levels` is top priority
- Sceptre for Spirit (Guiding Palm of the Eye, or rare with mana/+int/+spirit)
- Call of the Brotherhood — Lightning → Cold conversion, more Cold-Infusion gen
- Maligaro's Virtuosity + Quipolatl's Thesis — enables Pinpoint Critical without
  the crit damage downside; required for Cast on Critical setup

### End-game (Cast on Critical Comet)

Requirements:
- Enough Spirit (sceptre) to slot Cast on Critical
- High Critical Hit Chance (Pinpoint Critical on [[Spark]] + Maligaro's Virtuosity)
- **Cast on Critical MUST be the last gem in the gem list** — required for weapon
  swap to function

Setup:
- Cast on Critical → Comet
- Living Bomb (kept at minimum level for mana cost) → generates Fire-Infusions, which
  buff Comet damage by roughly 2x
- Elemental Weakness curse with Spell Cascade + Ritualistic Curse + Whispers of Doom
  passive
- Mana sustained via Pathfinder mana efficiency nodes + Quipolatl's Thesis

### Min-Max (optional chase)

- Headhunter (or Ingenuity as budget alternative)
- Palm of the Dreamer — Chaos Explosions on Spark; pairs with Tul's Stillness for freeze
- The Vertex corrupted with +2-4 Skill Gems — big damage, mana/tankiness cost
- Atziri's Splendour (CI only, must remove mana-to-life mod)
- Rite of Passage, The Fall of the Axe

## Weapon swap setup

- Weapon Set I (Wand): [[Spark]] — passive tree allocates Critical Hit Chance
- Weapon Set II (The Whispering Ice or staff): [[Frost Bomb]] — allocates Exposure
  Effect + Secrets of the Orb
- Skills auto-trigger on the correct weapon when configured via the in-game UI

## Stat priorities

**Offensive:**
- `+Spell Gem Levels` (majority of damage)
- Spell Damage
- Critical Strike Chance & Critical Damage Bonus
- Cast Speed
- Damage Gained as Lightning / Cold / Fire / Chaos
- Increased Duration
- Increased Projectile Speed

**Defensive:**
- Capped Fire / Cold / Lightning resistance
- Life (pre-CI)
- Evasion Rating
- Maximum Energy Shield
- Faster + Increased Energy Shield Recharge Rate

## Why this build for new players

- [[Spark]] usable from level 1, no special gear needed early
- Cold-Infusion loop is the only mechanic to learn for campaign
- Mobility from [[Pathfinder]] forgives positioning mistakes (cast-while-moving,
  no sprint stun, slow immunity)
- End-game CoC Comet + CI transition can be ignored until ready — campaign setup
  is self-contained
