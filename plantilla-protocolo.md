# Plantilla de protocolo — Experimento de ubicación de producto

**Equipo:** ___ · **Integrantes:** ___ · **Fecha:** 27/10/2026

Completa cada sección. Usa commits por sección; la historia del repositorio se revisa.

## 1. Pregunta e hipótesis

El producto en el pasillo principal vende más en promedio que en su ubicación habitual en ventas semanales durante 4 semanas.

## 2. Unidad experimental

Semana-Tienda (**# de tiendas por el # de semanas asociadas al experimento**)

-10 tiendas por 4 semanas = 40 unidades experimentales 

## 3. Factor, niveles y tratamiento

- **Factor** (variable manipulada): Ubicación
- **Niveles** (valores del factor): Pasillo y ubicación habitual
- **Tratamiento** (combinación asignada): Pasillo durante una semana y ubicación habitual durante otra (grupo de control)

## 4. Grupo de control

La misma tienda pero con el producto dispuesto en la ubicación habitual. 

## 5. Aleatorización

Sorteo de 20 tiendas a cada grupo (paralelo)
Explica por qué el sorteo reparte los factores desconocidos entre los grupos.

- **Línea de código de la asignación (Python o R):** escribe el comando que asigna al azar tus N unidades a los dos grupos (tratamiento y control) y ejecútalo con semilla. Incluye el resultado de una corrida y explica por qué el sorteo reparte los factores desconocidos entre los grupos.

## 6. Respuesta y medición

- Variable respuesta: Ventas semanales en USD
- Período de medición: 4 semanas 
- Quién registra y cómo (¿ciego?): Mediante el POS, ciego (vendedor no sabría si el producto está en principal o en habitual)

## 7. Factores a controlar (mínimo 4)

| Factor a controlar | Cómo se controla o registra |
|---|---|
| 1. | Clima |
| 2. | Evento Local|
| 3. | Surtido / Stock|
| 4. | Cambios en el personal|

## 8. Limitaciones del diseño

*¿Qué podría invalidar el experimento si no se controla? ¿Qué no se podrá concluir?*

- Pérdida de potencia por promociones
- Canibalización de las tiendas
- 

## 9. Comparación en código (Python/R)

*Escribe `scripts/comparacion_experimento.py` (o `.R`): debe cargar `plantillas/registro_experimento.csv` y calcular el promedio de `ventas_producto` por `ubicacion`. Incluye la salida y responde:*

- ¿Qué grupo muestra mayor venta promedio en la plantilla?
- ¿Por qué con 4 filas no se puede concluir nada sobre el efecto de la ubicación?
- Si el experimento se ejecutara con tu protocolo, ¿qué le faltaría a este análisis para ser justo?
