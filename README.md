# TP-Regresion-AA1-2025C2-Mezzano-Perez-Tapia

# Proyecto de Análisis de Datos y Modelado Predictivo

Este proyecto consiste en un análisis exploratorio y modelado predictivo sobre un dataset de viajes de Uber Inc en la ciudad de Nueva York. Incluye limpieza de datos, ingeniería de variables, imputación, análisis estadístico y comparación de modelos de regresión lineal y regularizados.

## Objetivo
Predecir el *fare amount* (precio del viaje) a partir de variables como distancia, tipo de día, turno y otras características derivadas, evaluando distintos enfoques de modelado.

## Contenido
- *Preprocesamiento de datos*: limpieza, eliminación de outliers, imputación (KNN para coordenadas faltantes), creación de variables dummies para turnos, feriados y días de semana.
- *Análisis exploratorio*: histogramas, análisis de correlaciones, gráficos de densidad.
- *Modelos*: regresión lineal, Ridge, Lasso, ElasticNet, entrenamiento con gradiente descendente, estocástico y mini-batch.
- *Evaluación*: RMSE, R², análisis de residuos.
- *Visualizaciones*: coeficientes de modelos, impacto de la regularización, comparación de errores.

## Resultados Clave
- La variable con mayor poder predictivo fue *distance_km*.
- Los modelos lineales clásicos (Regresión Lineal, Ridge, Lasso) mostraron rendimientos similares (RMSE ≈ 5.29, R² ≈ 0.71), indicando poca ganancia con regularización.
- Elastic Net mejoró el error (RMSE ≈ 4.51) manteniendo R² similar, logrando un balance más eficiente.
- Los métodos de optimización por gradiente descendente destacaron: Gradiente Descendente por Lotes y Mini-Batch obtuvieron los mejores resultados (RMSE ≈ 4.43–4.44, R² ≈ 0.77),
  mientras que el Gradiente Descendente Estocástico fue competitivo (RMSE ≈ 4.63, R² ≈ 0.75). 

## Librerías Utilizadas
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- holidays

## Uso
1. Clonar repositorio.
2. Cargar dataset.
3. Ejecutar scripts en orden: preprocesamiento → modelado → evaluación.
4. Revisar gráficas y métricas generadas.
