---
type: concept
patch: "0.4.0"
sources: [patch-0.4.0]
updated: 2026-05-21
tags: [bosses, mechanics, endgame]
---

# Boss Anti-Burst Damage Mechanic

Introduced in 0.4.0. Bosses gain a temporary damage reduction window after emerging or becoming aggro, discouraging instant-kill strategies.

## How it works

When a boss finishes emerging or becomes aggro, an anti-burst window begins:
- Damage reduction starts at full effect.
- Tapers to no effect over a fixed duration.
- Boss movement away from spawn location accelerates the falloff.
- Bosses that cannot or barely move have a shorter overall reduction window.

After the window expires, the boss takes full damage normally.

## Design intent

This appears targeted at builds that could one-shot bosses on emerge — typically high-burst spell combos, oversized crit chains, or pre-stacked debuffs. The mechanic forces the boss to "earn" its fight loop before it can be killed.

## Build implications

- **High-burst builds** (e.g. Lightning Conduit with stacked shock, Hexblast bomb setups, big Comet snipes) need to either wait out the window or sustain enough DPS through it.
- **Sustained DPS builds** (totems, minions, channeling skills, attack speed stacking) benefit relatively.
- **Boss positioning matters**: bosses that pace or charge (e.g. [[arbiter-of-ash]] post-0.4) drop reduction faster than stationary or slow bosses.

## Tactical play

- Open with mobility / setup rather than full commitment. Apply curses, debuffs, and ailments early.
- Force the boss to move if possible — the falloff accelerates with displacement.
- Pinnacle bosses with slow openings are now more punishing to "stand and unload" against.
- **Documented timing**: the [[Run n Gun Witchhunter]] build pre-stacks 4–5 Stormblast Bolts on the boss, then explicitly waits **~3 seconds** before dodge-detonating. The wait targets the anti-burst window — letting it taper before unloading prevents the initial reduction from wasting the stacked damage. This is the first documented build that deliberately times the rotation around this mechanic.

## Known affected bosses

The patch notes describe the mechanic as applying broadly to bosses with emerge or aggro animations. Specific tuning per boss is not documented in the patch notes. Empirical confirmation needed for individual bosses; file observations into this page as encountered.

## Open questions

- Exact duration of the full-effect window per boss tier.
- Whether the mechanic applies to map bosses or only pinnacle bosses.
- Interaction with damage-over-time effects (ailments, DOT) — does the reduction apply equally?
- Whether 0.5 modifies or removes this mechanic.

## See also

- [[arbiter-of-ash]]
- [[endgame-0.4.0]]
