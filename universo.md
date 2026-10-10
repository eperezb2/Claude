# Universo de emisores BVC

- **Fuente:** oanor screener (TradingView)
- **Fecha de consulta:** 10 de octubre de 2026
- **Resumen:** 30 confirmados · 5 pendientes · 4 excluidos
- **Aviso:** la fuente es un screener de TradingView sin clave, no la BVC. No usar en decisiones sin cruzar con la BVC.

Leyenda: `[VERIFICAR: ...]` marca un dato que no se recibió o que no se pudo confirmar. No se completó con supuestos.

## Confirmados (30)

[VERIFICAR: la lista de las 30 comunes y preferenciales no llegó en el mensaje; sin ella no se llenan las filas.]

| símbolo | emisor | tipo (común o preferencial) | estado | fuente | fecha de consulta |
|---|---|---|---|---|---|
| [VERIFICAR] | [VERIFICAR] | [VERIFICAR] | confirmado | oanor screener (TradingView) | 10 de octubre de 2026 |

Pendiente de completar: 30 filas. Recibidas: 0.

## Pendientes (5)

| símbolo | emisor | tipo (común o preferencial) | estado | fuente | fecha de consulta |
|---|---|---|---|---|---|
| CNEC | [VERIFICAR: emisor] | [VERIFICAR] | pendiente | oanor screener (TradingView) | 10 de octubre de 2026 |
| CXTESCOL | [VERIFICAR: emisor] | [VERIFICAR] | pendiente | oanor screener (TradingView) | 10 de octubre de 2026 |
| IBITCO | [VERIFICAR: emisor] | [VERIFICAR] | pendiente | oanor screener (TradingView) | 10 de octubre de 2026 |
| NUCO | [VERIFICAR: emisor] | [VERIFICAR] | pendiente | oanor screener (TradingView) | 10 de octubre de 2026 |
| PEI | [VERIFICAR: emisor] | [VERIFICAR] | pendiente | oanor screener (TradingView) | 10 de octubre de 2026 |

## Excluidos

| símbolo | motivo | origen del motivo |
|---|---|---|
| HCOLSEL | [VERIFICAR: motivo no indicado]. Hipótesis: instrumento de inversión colectiva (ETF) y no un emisor. | Inferencia, sin confirmar |
| ICOLCAP | [VERIFICAR: motivo no indicado]. Hipótesis: ETF que replica el COLCAP y no un emisor. | Inferencia, sin confirmar |
| NUAMCO | [VERIFICAR: motivo no indicado]. No hay base para suponerlo. | Sin dato |
| PFGRUPOARGOS | No encontrado: la API devolvió `found: false` el 10 de octubre de 2026 (sin `last`, `currency`, `volume` ni `name`) y tampoco aparece entre los 55 símbolos del screener. | Dato verificado en la consulta |

Nota sobre PFGRUPOARGOS: también se probaron `PFGRUPPARG` y `PFGRUPARG` el mismo día y ambos devolvieron `found: false`. No se confirmó el ticker oficial de la preferencial de Grupo Argos. [VERIFICAR: ticker en la BVC.]
