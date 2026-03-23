---
title: "Ciclo de cogeneración con turbina de vapor: dimensionamiento preliminar"
date: 2025-06-20
tags: [Cogeneración, Rankine, Turbina de vapor, CHP]
---

Notas sobre el procedimiento de dimensionamiento preliminar de un sistema de cogeneración basado en un ciclo Rankine con extracción de vapor para proceso.

## ¿Por qué cogeneración?

Un ciclo Rankine convencional de generación eléctrica tiene un rendimiento típico del 33-38%. La mayor parte de la energía del combustible se pierde como calor de rechazo en el condensador. Si ese calor puede aprovecharse para un proceso industrial, el rendimiento global del sistema puede superar el 80%.

## Configuraciones típicas

**Contrapresión (back-pressure):** Todo el vapor pasa por la turbina y sale a la presión requerida por el proceso. No hay condensador. Es la configuración más simple y eficiente, pero la generación eléctrica queda acoplada a la demanda de calor.

**Extracción-condensación:** Parte del vapor se extrae a presión intermedia para proceso y el resto se expande hasta el condensador. Ofrece mayor flexibilidad operativa a costa de mayor complejidad.

## Procedimiento de dimensionamiento

1. **Definir la demanda térmica:** Caudal de vapor de proceso, presión y temperatura requeridos
2. **Definir la presión de caldera:** Típicamente 40-60 bar para sistemas industriales medianos
3. **Calcular el salto entálpico disponible:** h_entrada - h_extracción
4. **Estimar la potencia eléctrica:** Ẇ = ṁ · Δh · η_turbina
5. **Verificar el balance energético global**
