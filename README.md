# Simulación de Monte Carlo para Evaluación de Estrategias de Inversión

Este proyecto utiliza simulaciones de Monte Carlo para analizar y comparar el comportamiento de dos estrategias de inversión con perfiles de riesgo distintos (conservadora y agresiva) a lo largo de un horizonte de 10 años.

## Objetivo

El objetivo principal es evaluar cómo la volatilidad y el retorno esperado impactan en el valor futuro de una inversión, modelando la incertidumbre a través de simulaciones estocásticas. Este enfoque permite medir cuantitativamente el riesgo y el potencial de ganancia de cada estrategia.

## Metodología

Se realizaron 10,000 simulaciones para cada cartera. En cada simulación, se proyectó el crecimiento de una inversión inicial de $10,000 utilizando retornos anuales aleatorios generados a partir de distribuciones normales con parámetros definidos para cada estrategia.

### Parámetros de las carteras simuladas:

| Cartera       | Retorno esperado anual | Volatilidad anual |
|---------------|------------------------|--------------------|
| Conservadora  | 5%                     | 8%                |
| Agresiva      | 9%                     | 25%               |

## Visualización comparativa

La siguiente gráfica muestra la distribución de resultados finales tras 10 años para ambas carteras:

![Comparación de carteras](img/comparacion_carteras.png)

## Métricas clave

Se calcularon métricas estadísticas relevantes para cada estrategia:

| Métrica                        | Conservadora | Agresiva |
|-------------------------------|--------------|----------|
| Valor esperado                | $16,318      | $23,759  |
| Mediana                       | $15,891      | $18,494  |
| Percentil 5 (Valor en Riesgo) | $10,453      | $4,607   |
| Percentil 95                  | $23,635      | $60,280  |
| Probabilidad de pérdida       | 3.35%        | 22.37%   |
| Probabilidad de duplicar      | 16.96%       | 46.05%   |

Estas métricas permiten comprender el balance entre riesgo y retorno, y son útiles para la toma de decisiones financieras fundamentadas.

## Cómo ejecutar el proyecto

1. Clona este repositorio en tu máquina local.
2. Instala las dependencias necesarias:

```bash
pip install -r requirements.txt
