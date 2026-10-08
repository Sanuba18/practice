# Caso de práctica: "TiendaCo" (retail colombiano)

**Tiempo sugerido:** 75 min (10 entender · 45 analizar · 20 presentar en el README)

## Contexto
TiendaCo es un retailer con tiendas físicas, app y web en 5 ciudades. El Gerente Comercial
siente que "las ventas se estancaron" y quiere decidir **dónde invertir el presupuesto de
marketing del próximo semestre**: ¿programa de lealtad, promociones o canal digital?

## Datos (`data/`)
- `clientes.csv`: customer_id, city, signup_date, segment, loyalty_member
- `transacciones.csv`: transaction_id, customer_id, date, category, channel, quantity, unit_price, discount_pct

Ingreso neto de una transacción = quantity × unit_price × (1 − discount_pct)

## Preguntas
1. **Calidad de datos:** ¿Qué problemas encuentras? ¿Cómo los tratas? Documenta tus supuestos.
2. **Tendencia:** ¿Cómo evolucionan las ventas netas mes a mes? ¿Es cierto que se estancaron?
3. **Drivers:** ¿Qué ciudades, categorías, canales y segmentos explican el ingreso?
4. **Lealtad:** ¿Los miembros del programa gastan más? ¿Es causal o puede haber sesgo?
5. **Clientes inactivos:** ¿Qué % de clientes no compra hace más de 90 días (al 30-jun-2025)? ¿Quiénes son?
6. **Recomendación:** ¿Dónde pondrías el presupuesto y por qué? Incluye un impacto estimado.

## Entregable
- Un notebook `analisis.ipynb` (o `analisis.py`) que corra de arriba a abajo sin errores.
- `README.md` con resumen ejecutivo, hallazgos y recomendación.
- **Al menos 3 commits** con mensajes claros y push a una rama `solucion` + Pull Request.

## Bonus (si sobra tiempo)
- Escribe la pregunta 3 en **SQL** (puedes usar `duckdb` o `sqlite3` sobre los CSV).
- Un gráfico que usarías en la slide principal para el gerente.
