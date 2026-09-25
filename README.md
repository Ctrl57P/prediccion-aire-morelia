# Predicción de Calidad del Aire en Morelia

## El Problema Social
Morelia enfrenta retos de salud pública debido a la contaminación del aire (quemas agrícolas, incendios forestales y aumento del parque vehicular). 
Las partículas PM2.5 están directamente ligadas a enfermedades respiratorias.

## El Objetivo del Proyecto
Desarrollar un modelo de predicción que permita anticipar los niveles de contaminación (PM2.5) con 24 horas de anticipación, basándose en el pronóstico del clima. Esto permitiría emitir alertas tempranas para que la población vulnerable evite actividades al aire libre.

## Fuentes de Datos Públicas a Utilizar
El modelo se entrenará cruzando dos bases de datos históricas:
1. **Datos de Contaminantes (PM2.5):** Extraídos del portal abierto del Sistema Nacional de Información de la Calidad del Aire (SINAICA - INECC) para las estaciones de Morelia.
2. **Datos Meteorológicos:** Histórico de temperatura (°C) y velocidad del viento (km/h) extraídos de las bases de datos de Open-Meteo / NASA POWER.

## Modelo a Implementar
Se utilizará un **Modelo de Regresión Lineal Múltiple**. 
* **Variables Independientes (Entradas):** Velocidad del viento, temperatura máxima, y día de la semana (proxy de tráfico vehicular).
* **Variable Dependiente (Salida):** Concentración promedio de PM2.5.
* **Visualización final:** Una gráfica de línea de tiempo comparando los niveles de contaminación reales vs. los predichos por el modelo, marcando la línea de "riesgo sanitario".
