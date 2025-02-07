# historico_AAPL_5_A-OS
El análisis de AAPL (2020-2024) muestra una tendencia alcista impulsada por lanzamientos y buenos resultados, con caídas en 2022-2023 por factores macroeconómicos. Herramientas técnicas y modelos predictivos (MAE: 5.89) fueron útiles. Se observó alta correlación con el PIB (0.89) y el CPI (0.81). Eventos clave influyen en el volumen
# Análisis de Precios de Acciones de Apple (AAPL)

Este proyecto realiza un análisis exhaustivo de los precios de las acciones de Apple (AAPL) desde 2020 hasta 2024, utilizando técnicas de Machine Learning y análisis económico. Se implementan modelos de regresión, incluyendo Random Forest y Redes Neuronales, así como un modelo ARIMA para predicciones a largo plazo.

## Contenido

1. **Importación de Bibliotecas**
   - Se utilizan bibliotecas como `yfinance`, `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`, y `keras`.

2. **Descarga de Datos**
   - Se descargan los datos históricos de precios de las acciones de Apple desde Yahoo Finance.

3. **Limpieza de Datos**
   - Se eliminan filas con valores faltantes y se añaden indicadores técnicos como la media móvil simple (SMA) y el índice de fuerza relativa (RSI).

4. **Visualización de Datos**
   - Se visualizan los precios históricos, las medias móviles, el RSI y el volumen de negociación.

5. **Preparación de Datos para Machine Learning**
   - Se define el objetivo como el precio de cierre del día siguiente y se preparan las características para el modelo.

6. **Modelos de Machine Learning**
   - **Random Forest Regressor**: Se entrena un modelo de Random Forest y se evalúa utilizando el error cuadrático medio (RMSE).
   - **Redes Neuronales**: Se construye y entrena un modelo de red neuronal para la predicción de precios.

7. **Predicciones a Largo Plazo con ARIMA**
   - Se ajusta un modelo ARIMA para realizar predicciones a largo plazo sobre los precios de las acciones.

8. **Análisis Económico**
   - Se descargan y analizan indicadores macroeconómicos como el PIB, el índice de precios al consumidor (CPI) y la tasa de interés de la Fed.
   - Se visualiza la relación entre el precio de las acciones de Apple y los indicadores macroeconómicos.

9. **Validación Cruzada y Ajuste de Hiperparámetros**
   - Se implementa validación cruzada para evaluar el rendimiento del modelo y se realiza un ajuste de hiperparámetros utilizando `GridSearchCV`.

## Resultados

- **Error Cuadrático Medio (RMSE)**:
  - Random Forest: 2.87
  - Red Neuronal: 9.10
  - Conclusión: El modelo de Random Forest tiene un mejor rendimiento.

- **Análisis de Correlación**:
  - El precio de Apple tiene una fuerte relación positiva con el PIB (0.89) y una relación débil con la inflación (0.80). La relación con la tasa de interés es moderada (0.68).

- **Mejores Parámetros para Random Forest**:
  - `max_depth`: 30
  - `n_estimators`: 100
  - Mejor puntuación: 175.95

## Requisitos

- Python 3.x
- Bibliotecas: `yfinance`, `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`, `keras`, `statsmodels`, `pandas_datareader`

## Ejecución

Para ejecutar el análisis, asegúrate de tener todas las bibliotecas instaladas y ejecuta el script en un entorno de Python.

```bash
pip install yfinance pandas numpy matplotlib seaborn scikit-learn keras statsmodels pandas_datareader
