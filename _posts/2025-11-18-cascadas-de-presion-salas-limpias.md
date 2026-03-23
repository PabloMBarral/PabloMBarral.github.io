---
title: "Cascadas de presión en salas limpias: errores comunes en el diseño"
date: 2025-11-18
tags: [HVAC, GMP, Salas limpias, ISPE]
---

Un análisis de los errores más frecuentes en el diseño de diferenciales de presión para instalaciones farmacéuticas GMP. Desde la subestimación de infiltraciones por aberturas de puertas hasta el dimensionamiento incorrecto de los dampers de sobrepresión, revisamos los puntos críticos que todo ingeniero HVAC debe considerar.

## El concepto de cascada de presión

En una instalación farmacéutica con salas limpias, la cascada de presión es el mecanismo principal para evitar la contaminación cruzada entre ambientes de distinta clasificación. El aire fluye siempre desde las zonas de mayor limpieza (mayor presión) hacia las de menor limpieza (menor presión).

El diferencial de presión típico entre salas adyacentes es de **12.5 a 15 Pa**, según la guía ISPE Baseline Vol. 2. Sin embargo, este valor de diseño no es universal — depende de la aplicación, el tipo de producto y la clasificación de las salas.

## Error #1: Subestimar las infiltraciones

El caudal de infiltración a través de una abertura se calcula como:

> Q̇ = Cd · A · √(2 · ΔP / ρ)

Donde `Cd` es el coeficiente de descarga (~0.65 para puertas), `A` es el área de la abertura, `ΔP` el diferencial de presión y `ρ` la densidad del aire.

El error más común es considerar únicamente las fugas estáticas (rendijas de puertas cerradas) y olvidar el efecto dinámico de la apertura de puertas. Una puerta estándar de 2.1 × 0.9 m abierta durante 5 segundos genera un intercambio de aire significativo que puede colapsar el diferencial de presión si el sistema no tiene la capacidad de respuesta adecuada.

## Error #2: Dampers de sobrepresión mal dimensionados

Los dampers de alivio de presión deben dimensionarse para mantener el diferencial de presión dentro del rango aceptable durante las perturbaciones (apertura de puertas, arranque de equipos). Un error frecuente es dimensionar el damper solo para el caudal nominal, sin considerar los transitorios.

## Error #3: No considerar el stack effect

En edificios de varios pisos, el efecto chimenea puede generar diferenciales de presión no intencionales que interfieren con la cascada de diseño. En climas con grandes diferencias de temperatura interior/exterior, este efecto puede ser del orden de 5-10 Pa por piso, suficiente para invertir la cascada en pisos superiores o inferiores.

## Recomendaciones de diseño

La clave para un diseño robusto de cascadas de presión es considerar todos los escenarios operativos — no solo el estado estacionario nominal. Esto incluye simulaciones de apertura de puertas, fallas de equipos, y variaciones estacionales de las condiciones exteriores.
