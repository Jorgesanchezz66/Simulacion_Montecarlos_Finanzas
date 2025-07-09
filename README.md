# Simulación de Monte Carlo para Evaluación de Estrategias de Inversión

Este proyecto aplica simulaciones de Monte Carlo para modelar y comparar el desempeño de dos carteras de inversión (conservadora y agresiva) a lo largo de un horizonte de 10 años.

## Objetivo

Evaluar el impacto de la incertidumbre en los retornos anuales sobre el valor futuro de una inversión, y cuantificar el riesgo asociado a distintos perfiles de riesgo/rentabilidad.

## Metodología

Se realizaron 10,000 simulaciones para cada estrategia con parámetros de retorno esperado y volatilidad diferenciados. Para cada simulación, se generaron trayectorias anuales utilizando distribuciones normales.

| Cartera       | Retorno Esperado | Volatilidad |
|---------------|------------------|-------------|
| Conservadora  | 5% anual          | 8%          |
| Agresiva      | 9% anual          | 25%         |

## Visualización

![Comparación de carteras](img/comparacion_carteras.png)

## Métricas clave

Las siguientes métricas resumen el comportamiento esperado de ambas estrategias:

- Valor Esperado
- Mediana
- Percentil 5 (Valor en Riesgo)
- Percentil 95
- Probabilidad de pérdida
- Probabilidad de duplicar la inversión

## Instrucciones

1. Clona este repositorio.
2. Instala las dependencias:

```bash
pip install -r requirements.txt
```

3. Ejecuta el notebook `simulacion_montecarlo.ipynb` paso a paso.

## Requisitos

- Python 3.8+
- Numpy
- Pandas
- Matplotlib
- Seaborn

## Estructura del proyecto

```
montecarlo_inversion_finanzas/
├── README.md
├── simulacion_montecarlo.ipynb
├── requirements.txt
└── img/
    └── comparacion_carteras.png
```

## Autor

Proyecto desarrollado como parte de un portafolio de análisis financiero aplicado a ciencia de datos.

