# Data Manager (APIs REST y colecciones)

## Objetivo
Conectar tu app a datos externos sin exponer secretos.

## Flujo (ASCII)
```
[Apphive UI] --(request)--> [Backend propio] --(secret/API Key)--> [Proveedor externo]
```

## Pasos
1. En tu backend crea un endpoint `/api/items` (GET/POST).
2. En Apphive, en **Data Manager**, agrega una **fuente** llamada `Items` → URL de tu backend.
3. Define **acciones**: `listItems`, `createItem`.
4. En UI, enlaza un **Repeater** a `listItems` y un **Form** a `createItem`.
5. Maneja estados: **loading**, **error**, **empty**.
