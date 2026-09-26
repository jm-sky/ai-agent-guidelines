# Linters / style

Źródło prawdy: **config w projekcie**. Tu: preferencje + przykłady z Gear Stack do kopiowania.

## Przykłady (`examples/gear-stack/`)

| Plik | Stack |
|---|---|
| [`eslint.config.ts`](examples/gear-stack/eslint.config.ts) | FE (Vue/TS) |
| [`.editorconfig`](examples/gear-stack/.editorconfig) | wspólne |
| [`pyrightconfig.json`](examples/gear-stack/pyrightconfig.json) | Python IDE |
| [`backend/pyproject.toml`](examples/gear-stack/backend/pyproject.toml) | black · ruff · mypy |

Skopiuj i dopasuj do projektu. Komendy (`pnpm lint`, `black`, …) → `AGENTS.md` projektu.

## Styl (zgodny z przykładami)

| TS / Vue | |
|---|---|
| bez `;` | single quotes |
| import sort (Perfectionist) | self-closing tags |
| max attr/line: 3 / 1 | unused OK z `_` |
| `} else {` w jednej linii | nie łamać przed else/catch/finally |

| Python | black + ruff + mypy (`line-length` 256 w przykładzie Gear Stack) |
|---|---|
