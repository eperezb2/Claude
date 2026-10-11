# Universo de emisores BVC

- **Fuente:** oanor screener (TradingView)
- **Fecha de consulta:** 10 de octubre de 2026 (las consultas de CNEC, CXTESCOL, IBITCO, NUCO y PEI se hicieron a las 19:15 hora de Colombia, 00:15 UTC del 11 de octubre)
- **Resumen:** 30 confirmados esperados (lista no recibida) + 2 confirmados verificados (CNEC, PEI) · 0 pendientes · 7 excluidos
- **Aviso:** la fuente es un screener de TradingView sin clave, no la BVC. No usar en decisiones sin cruzar con la BVC.

Leyenda: `[VERIFICAR: ...]` marca un dato que no se recibió o que no se pudo confirmar. No se completó con supuestos.

## Confirmados

### Confirmados por consulta a la API (2)

| símbolo | emisor | tipo (común o preferencial) | estado | fuente | fecha de consulta |
|---|---|---|---|---|---|
| CNEC | Canacol Energy Ltd. | [VERIFICAR: clase de acción] | confirmado | oanor screener (TradingView) | 10 de octubre de 2026 |
| PEI | Patrimonio Autonomo Estrategias Immobilarias | [VERIFICAR: parece patrimonio autónomo, no acción común ni preferencial] | confirmado | oanor screener (TradingView) | 10 de octubre de 2026 |

Notas:
- El emisor se tomó tal cual del campo `name` de la API (PEI viene con "Immobilarias" mal escrito en la fuente).
- CNEC: `last` COP 5.000 con `open`, `high` y `low` iguales y volumen 0. Parece un precio sin transacciones (inferencia). No trae `market_cap` ni `pe_ttm`.
- PEI: `last` COP 65.440, volumen 9.022, `market_cap` COP 2.823,2 mm, `pe_ttm` 4,811.

### Confirmados (30) según el mensaje del usuario

[VERIFICAR: la lista de las 30 comunes y preferenciales no llegó en el mensaje; sin ella no se llenan las filas. Tampoco se sabe si CNEC y PEI forman parte de esas 30.]

| símbolo | emisor | tipo (común o preferencial) | estado | fuente | fecha de consulta |
|---|---|---|---|---|---|
| [VERIFICAR] | [VERIFICAR] | [VERIFICAR] | confirmado | oanor screener (TradingView) | 10 de octubre de 2026 |

Pendiente de completar: 30 filas. Recibidas: 0.

## Pendientes

Ninguno. Los 5 pendientes originales se resolvieron el 10 de octubre de 2026 (hora de Colombia): CNEC y PEI pasaron a confirmados; CXTESCOL, IBITCO y NUCO pasaron a excluidos.

## Excluidos

| símbolo | motivo | origen del motivo |
|---|---|---|
| CXTESCOL | No encontrado: la API devolvió `found: false` (sin `last`, `currency`, `volume` ni `name`). No se sabe si el ticker está mal escrito o la fuente no lo cubre. [VERIFICAR: ticker en la BVC.] | Dato verificado en la consulta |
| IBITCO | No encontrado: la API devolvió `found: false`. [VERIFICAR: ticker en la BVC.] | Dato verificado en la consulta |
| NUCO | No encontrado: la API devolvió `found: false`. [VERIFICAR: ticker en la BVC.] | Dato verificado en la consulta |
| HCOLSEL | [VERIFICAR: motivo no indicado]. Hipótesis: instrumento de inversión colectiva (ETF) y no un emisor. | Inferencia, sin confirmar |
| ICOLCAP | [VERIFICAR: motivo no indicado]. Hipótesis: ETF que replica el COLCAP y no un emisor. | Inferencia, sin confirmar |
| NUAMCO | [VERIFICAR: motivo no indicado]. No hay base para suponerlo. | Sin dato |
| PFGRUPOARGOS | No encontrado: la API devolvió `found: false` el 10 de octubre de 2026 (sin `last`, `currency`, `volume` ni `name`) y tampoco aparece entre los 55 símbolos del screener. | Dato verificado en la consulta |

Notas:
- PFGRUPOARGOS: también se probaron `PFGRUPPARG` y `PFGRUPARG` el mismo día y ambos devolvieron `found: false`. No se confirmó el ticker oficial de la preferencial de Grupo Argos. [VERIFICAR: ticker en la BVC.]
- CXTESCOL, IBITCO y NUCO estaban pendientes y se movieron aquí por el resultado `found: false`, a partir de una sola consulta. Si el ticker real es otro, deben reevaluarse.
