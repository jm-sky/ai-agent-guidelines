# ai-agent-guidelines

Wspólne reguły dla agentów AI (Claude Code, Cursor, Hub).  
Nie trzymają stacku konkretnego projektu — to zostaje w `AGENTS.md` projektu.

## Dokumenty

| Plik | Temat |
|---|---|
| [communication.md](communication.md) | Intent, język, tempo, format odpowiedzi |
| [directory-structure.md](directory-structure.md) | `docs/`, nazwy plików, `AGENTS.md` |
| [linters.md](linters.md) | Preferencje + przykłady configów |
| [lifecycle.md](lifecycle.md) | Vision → plan → implement → review → verify |
| [planning.md](planning.md) | Wizja, roadmap, plan, implementation-notes |
| [review.md](review.md) | Sesje review i artefakty |
| [generators.md](generators.md) | Generatory na powtarzalną robotę |

## Przykłady

- [`examples/gear-stack/`](examples/gear-stack/) — configi do kopiowania (ESLint, EditorConfig, Pyright, Black/Ruff/Mypy)

## Jak używać

1. W projekcie trzymaj **`AGENTS.md`** (Claude Code już wspiera; cel: jeden plik wejściowy).
2. Linkuj do tego repo; lokalne wyjątki zostaw w projekcie.
3. Starsze `CLAUDE.md` / `.cursorrules` → migruj w stronę `AGENTS.md`.

**Statusy (docs):** `draft` · `todo` · `planned` · `in progress` · `done` · `verification needed`
