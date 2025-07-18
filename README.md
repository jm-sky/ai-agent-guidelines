# ai-agent-guidelines
Guidelines for Ai agents like Claude 

# 📘 Zasady dla agenta AI (Claude) – po rozpoczęciu projektu

## ✅ 1. Weryfikacja wersji technologii

Po rozpoczęciu nowego projektu:

1. Sprawdź, jakich technologii i wersji używa projekt (np. z pliku `stack.md`).
2. Porównaj te wersje z tymi, które znasz z treningu.
3. Jeśli projekt używa **nowszej wersji** niż ta, do której jesteś przyzwyczajony jako agent AI:
   - Dodaj informację o tym w repozytorium projektu (np. do pliku `CLAUDE.md` lub `compatibility.md`).
   - Od tego momentu **zawsze sprawdzaj dokumentację tej technologii**, zanim zaproponujesz kod lub rozwiązanie.
   - Nie opieraj się wyłącznie na swojej utrwalonej wiedzy — może być przestarzała.

📥 Przykład:
> Projekt: Laravel 12  
> Ty: Znajomość Laravel 10  
> 🔍 Sprawdź: https://laravel.com/docs/12.x

---

## ✅ 2. Rozpoznawanie wzorców i generatory

Po zapoznaniu się ze strukturą projektu i stylem implementacji:

1. Rozpoznaj wzorce, które będą stosowane w projekcie (np. CRUD, DTO + walidacja, resource API, CQRS, eventy domenowe).
2. Przygotuj **generatory plików lub szablonów** odpowiadające tym wzorcom, zgodne z konwencjami projektu.

### 🎯 Przykład: wzorzec CRUD (`Product`)

Generator powinien przygotować:

- Model lub typ danych (`Product.php`, `Product.ts`)
- `ProductController` lub `ProductService`
- Klasy walidujące (`StoreProductRequest`, `ProductFormSchema`)
- `ProductDTO` lub `ProductResource`
- (opcjonalnie) migrację, trasę, testy

Dobrze, jeśli generator bazuje na danych z pliku `domain-models.md`.

---

🎯 Cel wspólny dla obu zasad:
- Spójność
- Praktyczność
- Minimalizacja błędów wynikających z przestarzałych założeń lub ręcznego tworzenia powtarzalnych struktur
