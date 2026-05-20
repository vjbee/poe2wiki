# PoE 2 Wiki — Schema & Workflows

This is a personal knowledge wiki for Path of Exile 2 maintained by Claude Code.
The human curates sources and asks questions; Claude reads, writes, and maintains
every file under `wiki/`. Files under `raw/` are immutable.

## Folder layout

```
raw/
  articles/      # Clipped guides (maxroll, poewiki, Reddit posts)
  patches/       # Official patch notes
  videos/        # Video notes/transcripts (Zizaran, Pohx, Ghazzy, etc.)
  assets/        # Images (auto-downloaded by Obsidian)
wiki/
  skills/        # Active skill gems (one page per skill)
  supports/      # Support gems
  ascendancies/  # Ascendancy classes (Arcane Knight, Beastmaster, etc.)
  uniques/       # Unique items (Kah-Veer, Mjolnir, etc.)
  passives/      # Keystones, notable passives, cluster jewels
  concepts/      # Mechanics: damage types, scaling, defenses, life vs ES
  builds/        # Build archetypes & specific builds
  meta/          # Patch analysis, league state, tier lists over time
  sources/       # Summary page for each ingested source
index.md         # Catalog of all wiki pages (content-oriented)
log.md           # Chronological event log (append-only)
```

## Page conventions

Every wiki page starts with YAML frontmatter:

```yaml
---
type: skill | support | ascendancy | unique | passive | concept | build | meta | source
patch: "0.4.0" # patch the info reflects, when relevant
sources: [source-id-1, source-id-2] # which source pages contributed
updated: 2026-05-20
tags: [fire, totem, melee]
---
```

Use `[[wikilinks]]` for every reference to another entity/concept. Don't write
"Mighty Swing" — write `[[Mighty Swing]]`. This is what powers Obsidian's graph
view and makes the wiki actually useful.

When a claim depends on patch state, mark it: `(as of [[patches/0.4.0]])`.

## Source page template (sources/)

```markdown
---
type: source
source_type: article | video | patch | reddit
url: https://...
author: ...
date: 2026-05-20
patch: "0.4.0"
ingested: 2026-05-20
---

# {Title}

## TL;DR

2-4 sentence summary.

## Key claims

- Bullet of each major claim, with [[wikilinks]] to relevant entities
- Note anything that contradicts existing wiki pages

## Updated pages

- [[wiki/skills/Whirlwind]] — added scaling notes
- [[wiki/builds/Arcane Knight Whirlwind]] — created
```

## Workflows

### Ingest

When the human drops a new source into `raw/` and says "ingest this":

1. Read the source fully.
2. Discuss the 3-5 most important takeaways with the human BEFORE writing
   anything. Ask which to emphasize.
3. Create a `sources/<slug>.md` page using the template above.
4. Touch every relevant wiki page — create new ones for entities that don't
   exist yet, update existing ones with new info. Add `[[wikilinks]]` liberally.
5. If a new claim contradicts an existing page, DO NOT silently overwrite.
   Add a "Contested" section noting both versions and which source said what.
6. Update `index.md`.
7. Append to `log.md`: `## [YYYY-MM-DD] ingest | <Title>` followed by a short
   list of pages touched.

### Query

When the human asks a question:

1. Read `index.md` first to find relevant pages.
2. Read those pages. Follow `[[wikilinks]]` if needed.
3. Synthesize an answer with citations: `[[wiki/skills/Whirlwind]]`.
4. If the answer is substantial and novel, OFFER to file it as a new page
   (usually under `meta/` or `builds/`). Don't file automatically — ask.
5. Append to `log.md`: `## [YYYY-MM-DD] query | <one-line question>`.

### Lint

When the human says "lint" or "health check":

1. Find contradictions between pages.
2. Find stale claims (older patch tags than the current patch).
3. Find orphan pages (no inbound `[[wikilinks]]`).
4. Find entities mentioned in many pages but lacking their own page.
5. Suggest sources/questions to investigate next.
6. Append findings to `log.md` under `## [YYYY-MM-DD] lint`.

## Domain-specific notes

- **Patch sensitivity**: PoE 2 is in Early Access. Patches change everything.
  Every numeric claim (damage %, base values) MUST have a `patch:` tag.
- **Build pages** should link to every skill, support, unique, and keystone
  they use. Build pages are hubs in the graph.
- **Don't invent numbers**. If a source doesn't give exact values, write
  "scales with X" without making up percentages.
- **Skill vs Support**: Always disambiguate. "Mighty Swing" → support, not
  active skill.

## Quick conventions

- File names: kebab-case for multi-word (`arcane-knight.md`).
- Page titles: human readable (`# Arcane Knight`).
- Dates: ISO `YYYY-MM-DD`.
- Log entries always start with `## [YYYY-MM-DD] <op> | <subject>` so they
  parse with `grep "^## \[" log.md | tail -10`.
