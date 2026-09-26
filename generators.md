# Generators

| Cel | Powtarzalne wzorce → generator = mniej tokenów, mniej dryfu |
|---|---|
| 🟢 Kiedy | Ten sam układ plików ≥ 2× (np. CRUD) |
| 📥 Wejście | `domain`, `model` (+ opcjonalnie `domain-models.md`) |
| 📤 Wyjście | lista plików / ścieżek; kod dopiero po „chcę, abyś…” |

## Laravel

Inputs: domain, model

- Model — `App\\Domain\\[domain]\\Models\\[model]`
- Requests: Search, Store, Update
- DTO
- Resource
- CRUD controller

## Vue

- types — `model.type.ts`
- Service — `Model.service.ts`
- `useModel` + TanStack Query
- zod validation schema
- routes
- components: Model card, Add / Edit / Remove Modal
- pages: List / Add / Edit
