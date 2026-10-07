# Koszt i tokeny

Cel: **tanie, powtarzalne** użycie AI — uniknąć przepalania budżetu przez dryf scope, zbędny kontekst i budowanie od zera bez researchu.

## Hierarchia kosztów

| Tanio → drogo | Kiedy |
|---|---|
| 🛠️ Lokalne narzędzia (lint, test, docs w repo) | Powtarzalna / deterministyczna robota |
| 💬 Wąski chat + mały kontekst | Decyzja, plan, mała zmiana |
| 🎯 Jeden specjalista (rola) | Jasny scope (plan / kod / review) |
| ☁️ Cloud agent | Tylko gdy trzeba (quota!); nie na drobnostki |

## Kontekst

| ✅ | ❌ |
|---|---|
| Memory = trwałe reguły i mapy | Dump całego projektu co turn |
| Szczegóły epizodu w `docs/` | Profil zapchany draftami planów |
| Kompakt chatu + świeży ogon | Liczenie na „pamięta wszystko z stycznia” |

## Research przed budową

**Zanim coś tworzymy:** sprawdź, czy jest gotowiec, lepsze rozwiązanie albo uznany wzorzec (stack / internet) → krótki research → dopiero plan / kod.

| Szukamy | Po co |
|---|---|
| 📦 Gotowa lib / CLI / feature w stacku | nie pisać od zera |
| 🏆 Lepsze podejście | pushback + mniej iteracji |
| 📐 Wzorzec (docs, RFC, popularny projekt) | mniej wynajdywania koła |

### Limity źródeł

| | |
|---|---|
| 🎯 **Default** | ~**5** źródeł → wniosek / notatka w `docs/research/` |
| 📈 **Gdy trzeba** | do ~**10** (porównanie opcji, niejasny tradeoff, compliance) |
| 🛑 **Powyżej 10** | tylko ze świadomym OK / jasnym powodem (inaczej dryf kosztów) |

Research bez limitu („jeszcze 20 zakładek”) = anti-pattern.

## Workflow (oszczędza kasę)

1. Intent: „chcę X” = plan; kod dopiero na „abyś”.
2. Pushback na słabe pomysły — taniej niż zbudować złą rzecz 3× ([communication.md](communication.md)).
3. Research → plan w repo → implement ([lifecycle.md](lifecycle.md), [planning.md](planning.md)).
4. Generatory / szablony zamiast boilerplate z LLM ([generators.md](generators.md)).

## Anti-patterns

| 🔥 Pali tokeny | Zamiast tego |
|---|---|
| Rubber-stamp „świetny pomysł” | Krytyka + alternatywa / „nie robić” |
| 5 botów naraz na ten sam temat | Jeden wąski scope |
| AI jako `pnpm lint` w pętli | Lintery lokalnie |
| Cloud na każdą drobnostkę | Lokal / wąski chat |
| Research bez limitu | 5 (default) / do 10 |

## Checklist przed drogą akcją

- [ ] Da się bez LLM / bez cloud?
- [ ] Był research (gotowiec / wzorzec)?
- [ ] Scope wąski, jeden cel?
- [ ] Artefakt w `docs/` zamiast kolejnego wall of chat?
