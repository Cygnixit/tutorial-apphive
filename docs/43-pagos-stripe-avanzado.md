# Stripe avanzado — Payment Intents, 3DS, tarjetas y suscripciones

## Diagrama neutral
```
Apphive -> POST /payments/create-intent
<- clientSecret
Apphive -> confirm (3DS si aplica)
Webhook -> payment_intent.succeeded/failed
```

## Pasos (clic por clic)
1. Backend crea **PaymentIntent**.
2. Apphive confirma y muestra loader.
3. Webhook actualiza la orden.
4. Guardar tarjeta: `customer + setup intent`.
5. Suscripciones: `priceId`, `trial`, `invoice.payment_*`.
