# Log

## [2026-05-21] ingest | Cold Spark Pathfinder Build Guide (Maxroll, Goratha)

Source: `raw/articles/Cold Spark Pathfinder Build Guide.md` (patch 0.4.0).

Created (newcomer-focused minimal scope, 6 pages):

- [[wiki/sources/cold-spark-pathfinder-maxroll]]
- [[wiki/builds/cold-spark-pathfinder]]
- [[wiki/skills/spark]]
- [[wiki/skills/frost-bomb]]
- [[wiki/ascendancies/pathfinder]]
- [[wiki/concepts/cold-infusion]]

Updated: [[index.md]]

Deferred (mentioned in build page only, not yet pages of their own):

- Uniques: Maligaro's Virtuosity, Call of the Brotherhood, The Whispering Ice,
  Astramentis, Painter's Servant, Enfolding Dawn, Crown of the Victor, Grip of Kulemak,
  Guiding Palm of the Eye, Quipolatl's Thesis, Threaded Light
- Skills: Orb of Storms, Siphon Elements, Mana Remnants, Arctic Armour, Comet, Living Bomb
- Passives: Heavy Frost, Thin Ice, Secrets of the Orb, Path Seeker (covered in ascendancy page)
- Concepts: Cast on Critical mechanic, weapon-swap setup, Pinpoint Critical

Split into own pages once a second source covers them or a query needs them.

## [2026-05-21] ingest | Spiral Volley Deadeye Build Guide (Maxroll, Cptn_Garbage)

Source: `raw/articles/Spiral Volley Deadeye Build Guide.md` (patch 0.4.0).

Created (newcomer-focused minimal scope, 7 pages):

- [[wiki/sources/spiral-volley-deadeye-maxroll]]
- [[wiki/builds/spiral-volley-deadeye]]
- [[wiki/skills/spiral-volley]]
- [[wiki/skills/lightning-arrow]]
- [[wiki/skills/lightning-rod]]
- [[wiki/ascendancies/deadeye]]
- [[wiki/concepts/resonance]]

Updated: [[index.md]]

Cross-references with prior ingest:

- [[wiki/ascendancies/pathfinder]] is mentioned as an optional late-game respec target
- Maligaro's Virtuosity appears in both builds (crit enabler) — still deferred as a page

Deferred (mentioned in build page only):

- Uniques: Serpent's Egg, Cadiro's Gambit, Headhunter, Rigwald's Ferocity, Hyrri's Ire,
  Prism of Belief, Maligaro's Virtuosity (carry-over from prior ingest), Subterfuge Mask
- Skills: Snipe, Herald of Thunder, Wind Dancer, Tame Beast, Ghost Dance, Charge Regulation,
  Tornado Shot, Barrage, Freezing Salvo
- Supports: Armour Break III, Enduring Impact II, Perfected Endurance
- Passives: Far Shot, Leaping Ambush (anoint), Ambush, Charge Profusion II
- Concepts: weapon-swap mechanics, charge system (Endurance/Frenzy/Power overview)

No contradictions between the two sources — they cover disjoint playstyles within Ranger
(spell Pathfinder vs. bow Deadeye). Pathfinder ascendancy entry was authored from the
Cold Spark guide; the Spiral Volley guide adds context that Pathfinder works for bow
builds too via the 0.4.0 Running Assault knockdown buff.

## [2026-05-21] ingest | Patch 0.4.0 — The Last of the Druids

Source: https://www.pathofexile.com/forum/view-thread/3883495 (saved to `raw/patches/patch-0.4.0.md`)
Focus per user direction: endgame and meta — to establish a baseline diff target against 0.5.0.

**Pages created:**

- `wiki/sources/patch-0.4.0.md`
- `wiki/meta/endgame-0.4.0.md`
- `wiki/concepts/map-effectiveness.md`
- `wiki/concepts/tablet-crafting.md`
- `wiki/concepts/boss-anti-burst.md`

**Pages updated:**

- `index.md` (initial population)
- `log.md` (initial population)

**Notes:**

- First ingest. No contradiction checks possible — establishes ground truth.
- 17+ stub entities/concepts noted in index for future ingests (Druid, ascendancies, content layers, etc.).
- Timing: 8 days before 0.5.0 release; patch notes for 0.5 drop today. The `endgame-0.4.0` page is the primary artifact, designed for diff against 0.5.0.
- Out-of-scope sections from patch notes (Druid, gem/ascendancy/unique rebalances) left for follow-up ingests per user direction.
- Hotfixes 0.4.0a–d to be ingested as a separate source file.

**Suggested next ingests:**

- 0.4.0a–d hotfix consolidated notes
- 0.5.0 patch notes (when released today, May 21)
- A maxroll.gg build guide for an Arcane Knight or Beastmaster build (to start filling skill / build pages)

## [2026-05-21] lint | Schema consistency pass

Findings + fixes:

- **Misplaced files**: 3 pages with `type: concept` were under `wiki/builds/`. Moved via `git mv`:
  - `wiki/builds/boss-anti-burst.md` → `wiki/concepts/boss-anti-burst.md`
  - `wiki/builds/map-effectiveness.md` → `wiki/concepts/map-effectiveness.md`
  - `wiki/builds/tablet-crafting.md` → `wiki/concepts/tablet-crafting.md`
- **`index.md` cleanup**: removed duplicate Meta + Concepts sections; merged all 5 concept pages under a single Concepts section; unified wikilink style to basename-only (`[[map-effectiveness]]`) for catalog entries.
- **Wikilink style** (decided convention):
  - Catalog/content references → basename (`[[Spark]]`, `[[map-effectiveness]]`)
  - Source page "Pages created/Updated" lists → full path (`[[wiki/concepts/X]]`) per CLAUDE.md template
- **Link fixes applied**:
  - `wiki/sources/patch-0.4.0.md` — `[[concepts/X]]` → `[[wiki/concepts/X]]` in "Pages created"
  - `wiki/meta/endgame-0.4.0.md` — `[[sources/patch-0.4.0]]` → `[[patch-0.4.0]]`

No content changes; no contradictions surfaced.

## [2026-05-21] lint | Health check

**Patch staleness**: none — all 17 wiki pages tagged `patch: "0.4.0"`, matching current. 0.5.0 release on 2026-05-29 (8 days out) will flip every page into a diff candidate simultaneously.

**Orphans**: none. Every wiki page has ≥2 inbound wikilinks across basename and Title-Case variants. [[endgame-0.4.0]] is the largest hub (7 inbound).

**Promote candidates** (stub entities with high inbound count, no page yet):

| Entity | inbound | rationale |
| --- | --- | --- |
| `arbiter-of-ash` | 8 | Gateway boss for tablet-crafting slots 3–4; referenced by every endgame page |
| `liquid-emotions` | 4 | Delirium reward mechanic, replaces reward bar (0.4) |
| `atlas-passive-tree` | 4 | New Abyss section in 0.4; nav hub |
| `abyss` | 4 | Promoted to core in 0.4 |
| `waystone` | 3 | Foundational mapping item |

**Contradictions**: none detected. Only 3 ingested sources with disjoint scope.

**Coverage gaps**:

- No Druid / Beastmaster / Arcane Knight content (Ranger sub-classes only — 2 builds).
- No video sources ingested.
- 0.4.0a–d hotfixes still deferred from initial patch ingest.
- 0.5.0 patch notes imminent (release 2026-05-29).

**Wikilink style**: consistent after the schema lint pass earlier today.

**Suggested next actions**:

1. Promote [[arbiter-of-ash]] to a page (highest leverage — 8 inbound).
2. Ingest 0.4.0a–d hotfix consolidated notes before 0.5 drops.
3. On 2026-05-29: ingest 0.5.0 patch notes and diff against [[endgame-0.4.0]].
4. Source a non-Ranger build (Druid or Arcane Knight) to broaden coverage.

## [2026-05-21] promote | Arbiter of Ash

Promoted from stub to full page using facts already present in the wiki — no new raw source required.

Created: `wiki/concepts/arbiter-of-ash.md` (type: concept; bosses do not yet have their own type in the schema)

Updated:

- `index.md` — added under Concepts, removed from Stubs/Entities

Stitched from existing references in [[endgame-0.4.0]], [[tablet-crafting]], [[boss-anti-burst]], [[patch-0.4.0]]. Raw 0.4.0 patch notes scanned — no Arbiter facts beyond what was already captured in [[patch-0.4.0]].

Open questions logged on the page: exact phase-transition life threshold, role in 0.5.0.

Stub count: 17 → 16.

## [2026-05-21] ingest | Patch 0.4.0d Patch Notes Preview

Source: https://www.pathofexile.com/forum/view-thread/3905675 (saved to `raw/patches/patch-0.4.0d.md`)

WebFetch'd directly under the standing autonomy granted earlier today. Mid-cycle league + QoL patch (Jan 14, 2026). No tablet, atlas, ascendancy, or skill-tree balance changes.

**Pages created:**

- `wiki/sources/patch-0.4.0d.md`
- `wiki/concepts/slow-cap.md` — monsters cannot be slowed below 25% of base speed
- `wiki/concepts/fate-of-the-vaal-league.md` — promoted from stub; Atziri Temple loop, Holten, beacons
- `wiki/concepts/trial-of-chaos.md` — endgame trial with rotating bosses; 0.4.0d boss tuning logged
- `wiki/skills/spectral-fire.md` — now uses player stats; explosion does not double-dip damage modifiers

**Pages updated:**

- `wiki/meta/endgame-0.4.0.md` — added "Patch evolution within 0.4" section pointing to 0.4.0d
- `index.md` — added 4 new entries; removed `fate-of-the-vaal-league` from stubs; added 0.4.0d source

**Deferred / skipped:**

- Phantasmal Arrow targeting bug fix (no build using it yet).
- Smith of Kitava's Temper Weapon + Talisman clarification (one-line edge case).
- Character sheet armour/evasion/ES display, spirit reservation display, augment art (UX polish).
- Specific Trial of Chaos bosses (Bahlak, Uxmal, Vornas, Morvak, Quadrilla) — referenced from the trial-of-chaos page but no individual pages.
- Twenty-five bug fixes listed in the source.

**Other hotfixes left for later**: 0.4.0a, 0.4.0b, 0.4.0c, 0.4.0e all exist on the forum. 0.4.0d was the most substantive of the 0.4 mid-cycle patches; the rest are iterative fixes. Ingest if/when relevant.

Stub count: 16 → 15 (fate-of-the-vaal-league promoted).
