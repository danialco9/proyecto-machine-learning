# Online Retail II

Proyecto de Machine Learning del máster. Trabajé con el dataset Online Retail II, que tiene algo más de un millón de ventas de una tienda online británica, y la pregunta que quería responder era qué clientes tienen más probabilidad de volver a comprar.

Lo primero fue limpiar los datos. Había bastantes devoluciones, duplicados y ventas sin cliente asociado (casi un 23 %), así que al final me quedé con unas 779.000 filas. Después hice el análisis exploratorio: cómo se reparten las ventas, en qué meses y a qué horas se vende más, y qué países y productos facturan más. Reino Unido se lleva más del 80 % de la facturación y hay un pico muy claro en octubre y noviembre por la campaña de Navidad.

Para el modelo agrupé los datos por cliente (frecuencia de compra, gasto total, ticket medio, días desde la última compra...) y usé una fecha de corte: con lo que pasó antes entreno, y lo que pasó después me dice si el cliente volvió o no. Usé una regresión logística porque me interesaba poder explicar qué variables pesan más, y eso se ve directamente en los coeficientes.

El análisis completo está en `online_retail_II_EDA-complete.ipynb`. El otro notebook es la primera versión.

Para ejecutarlo:

```
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl jupyter
jupyter notebook online_retail_II_EDA-complete.ipynb
```
