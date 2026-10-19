# Online Retail II — Análisis exploratorio y modelo de recompra

Análisis de más de **1 millón de transacciones** de una tienda online (dataset *Online Retail II*) y modelo que estima la **probabilidad de que un cliente vuelva a comprar**.

## Qué incluye

1. **Calidad de datos**: nulos, duplicados, devoluciones y tipos. Tras la limpieza quedan 779k filas (73 % del original); el 22,8 % de las transacciones no tiene cliente asociado.
2. **Estadística descriptiva y visualizaciones**: distribuciones de facturación, cantidad y precio; serie temporal mensual; top países y productos; patrones por día y hora.
3. **Dataset por cliente**: métricas RFM (frecuencia, gasto total, ticket medio, recencia, nº de productos…).
4. **Modelo de recompra**: regresión logística con fecha de corte temporal (features antes del corte, etiqueta después) y búsqueda de hiperparámetros.
5. **Explicabilidad**: coeficientes y *odds ratios* para entender qué variables impulsan la recompra.
6. **Conclusiones de negocio**: 5.878 clientes en 41 países, Reino Unido ≈ 83 % de la facturación y pico de ventas en octubre-noviembre.

## Archivos

| Archivo | Descripción |
|---|---|
| `online_retail_II_EDA-complete.ipynb` | Análisis completo con modelo y conclusiones |
| `online_retail_II_EDA-basic.ipynb` | Versión inicial del EDA |
| `online_retail_II.xlsx` | Dataset |

## Tecnologías

Python · Pandas · NumPy · Matplotlib · Seaborn · scikit-learn · Jupyter

## Cómo ejecutarlo

```bash
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl jupyter
jupyter notebook online_retail_II_EDA-complete.ipynb
```

---
Proyecto del Máster en Data Science & IA (Evolve) · [Daniel Alconada](https://github.com/danialco9)
