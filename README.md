📊 Análisis de Empleabilidad por Provincia y Sector en Argentina
Tablero de Power BI que analiza las tendencias de empleo, la composición del sector y la volatilidad regional en Argentina utilizando datos históricos.



Evolución, estructura y volatilidad del empleo basada en datos históricos

📌 Objetivo del proyecto

El objetivo de este proyecto es analizar la evolución del empleo en Argentina a lo largo del tiempo, combinando información de:

cantidad total de puestos de trabajo

variación interanual del empleo

distribución geográfica por provincia

composición sectorial (CLAE2)

niveles de volatilidad

con el fin de identificar patrones estructurales, tendencias temporales y diferencias regionales, y traducirlos en insights claros mediante un dashboard interactivo desarrollado en Power BI.

El foco no está solo en “cuántos puestos hay”, sino en cómo cambian, dónde se concentran y qué tan estables son.

🧠 Preguntas clave que responde el dashboard

El dashboard fue diseñado para responder, entre otras, las siguientes preguntas:

¿Cómo evolucionó el empleo total a lo largo de los años?

¿Qué provincias concentran la mayor cantidad de puestos de trabajo?

¿Qué tan volátil es el empleo según la provincia?

¿Existen provincias con poco empleo pero alta inestabilidad?

¿Qué sectores económicos explican la mayor parte del empleo?

¿Cómo cambia el peso relativo de cada provincia a lo largo del tiempo?

¿La variación interanual acompaña o contradice el crecimiento del empleo?

Estas preguntas guían toda la estructura visual del dashboard.

🗂️ Dataset utilizado

El dataset contiene información histórica del empleo en Argentina, desagregada por:

Año

Provincia

Sector económico (CLAE2)

Cantidad de puestos de trabajo

A partir de estos datos se calcularon métricas derivadas como:

variación interanual del empleo

volatilidad interanual

participación relativa por provincia

El volumen y la granularidad del dataset permiten realizar análisis:

temporales

comparativos

estructurales

exploratorios

🔧 Herramientas y tecnologías utilizadas

Power BI

Power Query para:

limpieza de datos

estandarización de categorías

transformación temporal

DAX para:

cálculo de variación interanual

métricas agregadas

volatilidad promedio

rankings dinámicos

Modelado de datos orientado a análisis y storytelling

📊 Estructura del dashboard (🔹) y decisiones de diseño (👉)
🔹 KPIs principales

En la parte superior del dashboard se presentan indicadores clave:

Cantidad total de puestos de trabajo

Provincia con mayor cantidad de puestos

Volatilidad interanual promedio

Distribución de puestos por sector

👉 Estos KPIs permiten obtener contexto inmediato antes de profundizar en el análisis y funcionan como punto de referencia para interpretar el resto de los gráficos.

🔹 Mapa de calor de variación interanual por provincia

Tabla tipo heatmap que muestra la variación interanual del empleo por provincia y año.

👉 Permite:

detectar ciclos de crecimiento y contracción

identificar años críticos

comparar rápidamente comportamientos regionales

visualizar estabilidad vs inestabilidad a lo largo del tiempo

El uso de colores facilita la lectura sin necesidad de interpretar cada valor numérico.

🔹 Evolución anual del empleo y variación interanual

Gráfico combinado de barras y línea:

Barras: cantidad total de puestos por año

Línea: variación interanual

👉 Este gráfico es el eje temporal del dashboard y permite:

observar tendencias de largo plazo

identificar quiebres estructurales

relacionar crecimiento absoluto con cambios relativos

Es clave para entender qué pasó y cuándo pasó.

🔹 Relación entre tamaño del empleo y volatilidad por provincia

Scatter plot que cruza:

Eje X: cantidad total de puestos

Eje Y: volatilidad interanual

Color: provincia

👉 Este gráfico permite identificar:

provincias grandes y estables

provincias pequeñas pero volátiles

casos atípicos que requieren análisis adicional

Aporta una dimensión de riesgo y estabilidad que no se observa en gráficos tradicionales.

🔹 Peso relativo de cada provincia por año

Gráfico de barras apiladas que muestra cómo se distribuye el empleo entre provincias a lo largo del tiempo.

👉 Permite:

analizar concentración del empleo

detectar cambios en la participación relativa

entender dinámicas estructurales más allá del crecimiento total

Es especialmente útil para análisis comparativos de largo plazo.

🔹 Cantidad de puestos por sector (CLAE2)

Gráfico de barras horizontales que muestra los sectores con mayor cantidad de puestos.

👉 Facilita:

identificar sectores clave del empleo

entender la estructura productiva

contextualizar los resultados geográficos y temporales

🚀 Conclusiones principales

El empleo presenta una fuerte concentración en pocas provincias.

El crecimiento del empleo no siempre implica mayor estabilidad.

Existen provincias con bajo volumen pero alta volatilidad.

La variación interanual permite identificar ciclos económicos claros.

La composición sectorial explica gran parte del comportamiento agregado.
