# Analisis_desempeño_logistica

Objetivo: Analizar datos históricos de entregas para identificar:

Tiempos promedio de entrega.
Retrasos frecuentes por región, conductor o tipo de paquete.
Cumplimiento de tiempos de entrega en comparación con los objetivos establecidos.

## Herramientas y tipo de proyecto

![Static Badge](https://img.shields.io/badge/sklearn-blue?style=for-the-badge)
 | ![Static Badge](https://img.shields.io/badge/pandas-blue?style=for-the-badge&logo=pandas)
 | ![Static Badge](https://img.shields.io/badge/matplotlib.pyplot-blue?style=for-the-badge)
 | ![Static Badge](https://img.shields.io/badge/seaborn-blue?style=for-the-badge)
 | ![Static Badge](https://img.shields.io/badge/ETL-blue?style=for-the-badge)| 

## Metodología
- **Preprocesamiento de datos:**
Se verificaron y limpiaron los valores ausentes y duplicados.

- **Analisis Exploratorio de datos (EDA):**

Tiempo promedio de entrega.
Porcentaje de entregas a tiempo.
Porcentaje de entregas retrasadas por región o conductor.

## Visualizaciones destacadas
**Gráficos de barras para regiones con más retrasos.**  

![image](https://github.com/user-attachments/assets/5da65f5e-483d-43ac-a1fe-125ceefd7709)

En este grafico la región sur pareciera la región con más retrasos, sin embargo, también es la región con más entregas. Por otro lado la región Oeste tiene menor cantidad de entregas y un porcentaje mayor de retrasos.


**Histogramas de duración de entregas.** 

![image](https://github.com/user-attachments/assets/b99b63c6-eb87-4bdd-b7a3-5849be551028)

Como se puede observar la mayoria de las entregas se realizan antes de las 30 horas, lo que comparando con politicas de DHL son 1-2 días habiles por lo que nuestro servicio se encuentra dentro de lo esperado, sin embargo, como vimos en los otros gráficos tenemos un porcentaje de retrasos elevados que debemos atender.

**Líneas de tiempo para observar tendencias mensuales.**  

![image](https://github.com/user-attachments/assets/4c01bcc3-6add-4031-bfc4-b04af27b492f)

Podemos observar lo siguiente:

Los valles representan los días con menos entregas y rutas más eficientes
Los picos son los días de mayor demanda Como podemos observar los valles se concentran en los días miercoles para el dia 11 y 18. Hay fluctuaciones significativas durante el mes, disminuyendo durante los ultimos días del mes.
Hay una epoca estacional correspondiente a la navidad donde el número de entregas parece estabilizarse.


## Conclusiones y recomendaciones

Logramos observar que el porcentaje de retraso de los pedidos se encuentra en el 25% lo cual esta en el limite de lo aceptable durante las temporadas altas como lo es navidad. A su vez, tenemos el evento de Black friday del mes de noviembre y la navidad que son eventos importantes para envios, por lo que eso explica nuestros aumentos durante el inicio y el final del mes.

Por otro lado, analizando cada región, se logro observar que la región sur es la más eficiente aun con un mayor número de pedidos a comparación de la región oeste que tiene el menor número de entregas y el tiempo medio de duración más alto, convirtienedose en la región menos eficiente.

Recomendaciones: Para el primer caso:

Se tiene un porcentaje de retraso considerable, por lo que se sugiere contratar personal temporal para la temporada de diciembre. Usar servicios de terceros para entregas más lejanas. Para el segundo caso:
Capacitar al personal que traza las rutas.
Contratar más conductores para las regiones más grandes.
Generar indicadores como km recorrido por entrega realizada, con el fin de evaluar las rutas y la eficiencia del conductor.
