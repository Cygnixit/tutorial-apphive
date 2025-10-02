# Mercado Pago — Marketplace (split payments)

## Flujo
```
Seller OAuth -> guardas token
Compra -> preference con application_fee + collector_id del seller
Webhook -> confirma pago, registra fee
```
