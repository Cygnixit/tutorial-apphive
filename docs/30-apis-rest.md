# APIs REST (backend propio)

## Reglas básicas
- La app **no** guarda secretos.
- El backend firma/valida requests a terceros.
- Maneja **idempotencia** con `Idempotency-Key`.

## Endpoints ejemplo (pseudocódigo)
```
GET  /orders?tenantId=...
POST /orders     (valida esquema, crea, audita)
GET  /orders/:id
```
