## 📊 Análisis de Empleabilidad por Provincia y Sector en Argentina

Tablero de Power BI que analiza las tendencias de empleo, la composición del sector y la volatilidad regional en Argentina utilizando datos históricos.

Evolución, estructura y volatilidad del empleo basada en datos históricos

<img width="1460" height="808" alt="Captura de pantalla 2026-03-29 221314" src="https://github.com/user-attachments/assets/687dbd04-ee55-40a5-8b2f-e4dde656d196" />


## 📌 Objetivo del proyecto

El objetivo de este proyecto es analizar la evolución del empleo en Argentina a lo largo del periodo 2007-2023, tomando como base la información extraida de la página datos.gob.ar, la misma publica la información en base al Ministerio de Desarrollo Productivo y tomando como fuente primaria la Administración Federal de Ingresos Públicos (AFIP)(https://datos.gob.ar/dataset/produccion-puestos-trabajo-asalariados-registrados-por-provincia-sector-actividad).
En esta base de datos se combinan:

cantidad total de puestos de trabajo

variación interanual del empleo

distribución geográfica por provincia

composición sectorial (CLAE2)

niveles de volatilidad

con el fin de identificar patrones estructurales, tendencias temporales y diferencias regionales, y traducirlos en insights claros mediante un dashboard interactivo desarrollado en Power BI.

El foco no está solo en “cuántos puestos hay”, sino en cómo cambian, dónde se concentran y qué tan estables son.

## 🧠 Preguntas clave que responde el dashboard

El dashboard fue diseñado para responder, entre otras, las siguientes preguntas:

¿Cómo evolucionó el empleo total a lo largo de los años?

¿Qué provincias concentran la mayor cantidad de puestos de trabajo?

¿Qué tan volátil es el empleo según la provincia?

¿Existen provincias con poco empleo pero alta inestabilidad?

¿Qué sectores económicos explican la mayor parte del empleo?

¿Cambia el peso relativo de cada provincia a lo largo del tiempo o siempre son las mismas provincias las que concentran la mayor cantidad de empleo?

¿La variación interanual acompaña o contradice el crecimiento del empleo?

Estas preguntas guían toda la estructura visual del dashboard.

## 🗂️ Dataset utilizado

El dataset contiene información histórica del empleo en Argentina, desagregada por:

Tabla 1:

Fecha

Provincia

Sector económico (CLAE2)

Cantidad de puestos de trabajo

Tabla 2:

CLAE6

descripción CLAE6

CLAE3

descripción CLAE3

CLAE2

descripción CLAE2

letra

descripción letra

A partir de estos datos se agregaron las columnas "año" en la Tabla 1 y "Rubro" en la Tabla 2, y se calcularon métricas derivadas que fueron ingresadas en una tabla aparte para una mejor práctica y con sus correspondientes descripciones. 
Las mismas serían:

variación interanual

volatilidad 

participación por provincia

porcentaje de representatividad por provincia 

puestos año actual

El volumen y la granularidad del dataset permiten realizar análisis:

temporales

comparativos

estructurales

exploratorios

## 🔧 Herramientas y tecnologías utilizadas

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

## 📊 Estructura del dashboard (🔹) y decisiones de diseño (👉)

## 🔹 KPIs principales

En la parte superior del dashboard se presentan indicadores clave:

Cantidad total de puestos de trabajo

Provincia con mayor cantidad de puestos

Volatilidad interanual promedio

Distribución de puestos por sector

👉 Estos KPIs permiten obtener contexto inmediato antes de profundizar en el análisis y funcionan como punto de referencia para interpretar el resto de los gráficos.

## 🔹 Mapa de calor de variación interanual por provincia

Tabla tipo heatmap que muestra la variación interanual del empleo por provincia y año.

👉 Permite:

detectar ciclos de crecimiento y contracción

identificar años críticos

comparar rápidamente comportamientos regionales

visualizar estabilidad vs inestabilidad a lo largo del tiempo

El uso de colores facilita la lectura sin necesidad de interpretar cada valor numérico.

## 🔹 Evolución anual del empleo y variación interanual

Gráfico combinado de barras y línea:

Barras: cantidad total de puestos por año

Línea: variación interanual

👉 Este gráfico es el eje temporal del dashboard y permite:

observar tendencias de largo plazo

identificar quiebres estructurales

relacionar crecimiento absoluto con cambios relativos

Es clave para entender qué pasó y cuándo pasó.

## 🔹 Relación entre tamaño del empleo y volatilidad por provincia

Scatter plot que cruza:

Eje X: cantidad total de puestos

Eje Y: volatilidad interanual

Color: provincia

👉 Este gráfico permite identificar:

provincias grandes y estables

provincias pequeñas pero volátiles

casos atípicos que requieren análisis adicional

Aporta una dimensión de riesgo y estabilidad que no se observa en gráficos tradicionales.

## 🔹 Distribución porcentual del empleo por provincia

Gráfico de barras apiladas que muestra cómo se distribuye el empleo entre provincias a lo largo del tiempo.

👉 Permite:

analizar concentración del empleo

detectar cambios en la participación relativa

entender dinámicas estructurales más allá del crecimiento total

Es especialmente útil para análisis comparativos de largo plazo.

## 🔹 Top sectores por cantidad de puestos de trabajo

Gráfico de barras horizontales que muestra los sectores con mayor cantidad de puestos.

👉 Facilita:

identificar sectores clave del empleo

entender la estructura productiva

contextualizar los resultados geográficos y temporales

## 🎯 Decisiones de Diseño

¿Por qué no hay mapa geográfico?
Evalué incluir un mapa de calor de Argentina, pero decidí que:
- El scatter plot de tamaño vs volatilidad aporta más insight analítico
- La matriz de variación interanual es más precisa para comparaciones
- Un mapa solo confirmaría lo obvio (Buenos Aires domina)

¿Por qué barras 100% apiladas?
Porque permiten ver cambios en participación relativa de provincias más 
pequeñas, que serían invisibles en valores absolutos dominados por Buenos Aires.

¿Por qué volatilidad como métrica?
La volatilidad (desviación estándar de variación interanual) identifica 
provincias con empleo inestable vs estable, útil para evaluar riesgo económico.

## 🚀 Conclusiones principales

El empleo presenta una fuerte concentración en pocas provincias, más precisamente en Buenos Aires y Capital Federal.

El crecimiento del empleo no siempre implica mayor estabilidad.

Existen provincias con bajo volumen pero alta volatilidad como Tierra del Fuego y Catamarca.

La variación interanual permite identificar ciclos económicos claros, es algo que se puede visualizar claramente en el periodo 2019 y 2020 donde casi todas las provincias tuvieron caídas en el empleo devido a la pandemia de COVID; salvo Capital Federal, el resto de las provincias del país muestran un crecimiento interanual del empleo en el periodo de 2008 a 2015 pero luego de este año, en el periodo 2015 a 2023, la tendencia se invierte y las mayorias de provincias registran retrocesos laborales.

La composición sectorial explica gran parte del comportamiento agregado, es decir, la evolución del empleo agregado está fuertemente influenciada por los sectores con mayor participación en el total, lo que indica que cambios en estos sectores dominantes explican gran parte de la dinámica general del mercado laboral, estos serían Comercio al por menor excepto autos y motos, Enseñanza, Comercio al por mayor excepto autos y motos y Agricultura, ganadería, caza y servicios relacionados.

El sector de Servicios es el que más puestos de trabajo representa, muy por encima de los sectores Primario e Industrial, marcando un peso porcentual de casi un 73%.
