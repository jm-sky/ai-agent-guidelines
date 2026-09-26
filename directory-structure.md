# Struktura katalogów

## Agent entry

| Cel | Jeden plik **`AGENTS.md`** w root projektu (Claude Code wspiera) |
|---|---|
| Migracja | `CLAUDE.md` / `.cursorrules` → `AGENTS.md` |

Lokalne wyjątki i komendy projektu zostają w `AGENTS.md` projektu. Wspólne reguły → to repo.

## `docs/`

| Katalog | Po co |
|---|---|
| 📁 `vision/` | wizja / kierunek |
| 📁 `roadmap/` | roadmapy (większy zakres) |
| 📁 `plans/` | plany implementacji |
| 📁 `plans/implementation-notes/` | wytyczne pod implementację (ścieżki, symbole) |
| 📁 `reviews/` | sesje review |
| 📁 `research/` | spike / porównania przed decyzją |
| 📁 `issues/` | błędy, dług, usprawnienia |
| 📁 `performance/` | perf notes / pomiary |
| 📁 `archive/` | stare docs |

## Nazwy plików

| Rodzaj | Wzorzec |
|---|---|
| Review | `YYYY-MM-DD--001--temat.md` (ID: 3 cyfry) |
| Plan (większe projekty) | `domain--id--title.md` |
| Issues / inne | `YYYY-MM-DD--NNN--slug.md` (gdy pasuje) |

## Nagłówek planu

```markdown
# title

**Status:** `draft`
**Created:** -
**Domain:** -
**Roadmap:** -
**Depends on:** -
**Finished:** -

Content...
```

Nagłówek pod skrypty: lista planów i zależności.

## Statusy

`draft` · `todo` · `planned` · `in progress` · `done` · `verification needed`
