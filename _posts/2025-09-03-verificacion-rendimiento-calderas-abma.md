---
title: "Verificación de rendimiento en calderas humotubulares: método ABMA"
date: 2025-09-03
tags: [Calderas, ABMA, Rendimiento, Tecnología del Calor]
---

Una guía paso a paso para verificar el rendimiento de calderas de vapor usando el método de pérdidas indirectas según las directrices ABMA.

## Método directo vs. indirecto

El rendimiento de una caldera puede determinarse por dos caminos: el método directo (input-output) mide la energía entregada al vapor y la energía suministrada por el combustible; el método indirecto cuantifica cada una de las pérdidas individuales y las resta del 100%.

En la práctica industrial, el **método indirecto** es preferido porque permite identificar la contribución de cada pérdida, requiere menos instrumentación de precisión y es más robusto frente a incertidumbres de medición de caudal.

## Las pérdidas principales

Para una caldera a gas natural, las pérdidas típicas son:

**Pérdida por gases secos** — Es la pérdida dominante (4-8%). Depende de la temperatura de chimenea y el exceso de aire.

```python
def perdida_gases_secos(T_chimenea, T_amb, CO2_pct):
    """Pérdida porcentual por gases secos según ABMA."""
    K = 0.56  # Factor para gas natural
    return K * (T_chimenea - T_amb) / CO2_pct
```

**Pérdida por humedad del combustible** — El hidrógeno del gas natural genera agua de combustión que se pierde como vapor en los gases de escape (~10-11%).

**Pérdida por radiación y convección** — Depende del tamaño de la caldera y su aislación. Típicamente 0.5-1.5%.

## Ejemplo numérico

Para una caldera humotubular de 10 ton/h quemando gas natural con una temperatura de chimenea de 220°C y 3% de O₂ en gases:

- Pérdida por gases secos: ~5.2%
- Pérdida por humedad del combustible: ~10.8%
- Pérdida por humedad del aire: ~0.3%
- Pérdida por radiación: ~0.8%
- **Rendimiento = 100 - 17.1 = 82.9%**
