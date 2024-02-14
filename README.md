# Análisis De Siniestros Viales en la Ciudad De Buenos Aires, Argentina
Realizado por: Cristian Silva

En este proyecto, se busca realizar un análisis exhaustivo de los datos relacionados con los siniestros viales ocurridos en la Ciudad de Buenos Aires entre los años 2016 y 2021. El propósito principal es proporcionar a las autoridades locales información detallada y precisa que les permita tomar medidas concretas para reducir el número de víctimas fatales causadas por estos incidentes.

## Contexto:

Los siniestros viales se definen como cualquier evento o incidente que ocurre en las vías públicas e involucra vehículos de motor, peatones o ciclistas, resultando en daños materiales, lesiones o pérdida de vidas humanas. Este fenómeno ha llevado a diversas regiones a mantener registros detallados de las tasas de mortalidad asociadas con los siniestros viales, con el objetivo de reducir dichas cifras mediante la implementación de medidas que abarcan desde la educación vial, hasta la mejora de la infraestructura y la promoción de vehículos seguros.

En el caso particular de la ciudad de Buenos Aires, emerge una preocupación significativa frente a este tipo de sucesos, dado su carácter de metrópolis con un tráfico intenso y una alta densidad poblacional. Según revela el Sistema Nacional de Información Criminal (SNIC), entre los años 2018 y 2022 se contabilizaron 19,630 muertes a causa de siniestros viales, lo que representa un promedio de 11 personas fallecidas diariamente en tales circunstancias. Estos incidentes no solo implican un riesgo para la seguridad de los habitantes de la ciudad, sino que también afectan la infraestructura urbana y la capacidad de los servicios de emergencia para responder eficazmente.

Por tanto, la importancia de un proyecto de esta envergadura radica en su capacidad para no solo llevar un seguimiento detallado de las estadísticas, sino también para evaluar y poner en práctica políticas destinadas a mitigar este problema de manera efectiva.

## Tecnologías utilizadas
Para el desarrollo de este proyecto se utilizaron las siguientes tecnologías: Phyton 3.10, Pandas, NumPy, Warnings, GeoPy, matplotlib, seaborn, spicy, GoogleSheets y tableau. 

## Metodología

### ETL

Se realizó un proceso ETL (Extracción, transformación y carga) en el cual se realizó una visualización inicial, se estandarizaron variables, se realizó una limpieza de datos mediante el analisis y eliminación de nulos, revisión y eliminación de duplicados y eliminación columnas redundantes al unificar los datasets. Luego de realizados estos procesos se evalúan los KPIs mediante sus formulas matemáticas. 

### EDA

A partir de los datos transformados y unificados, se realizó un EDA (Análisis exploratorio de datos), para ello se vizualizaron medidas globales de las cuales se analizaron comportamientos recurrentes en víctimas y accidentes a partir de los siguientes criterios:
- Demográficos:
   - Cantidad de víctimas fatales por año discriminadas por sexo.
   - Cantidad de víctimas fatales por año según su sexo y rango de edad.
   - Víctimas fatales según el vehículo que ocupaban.
   - Víctimas fatales según el vehículo que ocupaban y sexo.
   - Distribución de víctimas según el rol
   - Distribución de víctimas según el rol, discriminadas por sexo
   - Distribución según los participantes en los accidentes
- Espaciales:
   - Accidentes según el tipo de vía
   - Accidentes por comuna
- Temporales:
   - Número total de víctimas fatales por año
   - Distribución de víctimas fatales por mes
   - Distribución de víctimas fatales por mes, gráficos anuales comparados
   - Distribución de los accidentes con victimas fatales día por día a lo largo del mes
Cabe mencionar que en esta sección se tuvieron en cuenta los outliners para hacer análisis.
### Dashboard

Teniendo en cuenta los resultados del EDA, se realiza un Dashboard interactivo en Tableau, con el fin de presentar los datos de forma amigable para cualquiera fuera del mundo de la programación y el análisis de datos.

## Análisis

### Distribución temmporal de las víctimas

- El año con menos víctimas de siniestros viales fue el 2020, se asume que esto sucedió debido a los confinamientos preventivos por el Covid-19. 
- El año con más accidentes fue el 2018, debido a que no hay una causa aparente es necesario analizar políticas públicas implementadas en esta época y afectaciones climaticas que pudiesen dificultar la conducción.
- Se observa un pico notorio en la cantidad de víctimas fatales durante el més de diciembre, como hipótesis, los accidentes pueden aumentar debido a las festividades y el consumo de alcohol en las mismas.
- Noviembre y agosto también presentan un a cantidad notablemente más alta de accidentes fatales.
- Al comparar año a año la distribución de accidentes con victimas fatales por mes, no se observa tanta consistencia en un patrón que relacione la accidentalidad según los meses del año.

### Distriución demográfica de las víctimas

- Se evidencia que la cantidad de hombres que fallecen en un accidente de tránsito es mucho mayor que la cantidad de mujeres. Es pertinente evaluar y contrastar tipos de vehículos, roles y participación en estos accidentes.
- Fueron pocas las victimas fatales menores de 15 años y mayores de 80, en el caso de estas últimas se encuentran como outliers en los años 201,2017 y 2019. 
- La mayoría de víctimas se encuentran entre los 16 y los 45 años de edad.
- Los motociclistas y los peatones son más vulnerables a fallecer en un accidente vial. Estos datos proporcionan ua guía de hacia quien deberían encaminarse las campañas de prevención.
- Los conductores tienen más víctimas fatales, seguidos por los peatones. Es pertinente evaluar la seguridad de los vehículos y su relación con la muerte del conductor.

### Distribuvión espacial

- La accidentalidad es más alta en las avenidas en comparación con otros tipos de vía. Se hipotetiza que esto se debe a que en la Avenida, la velocidad de los conductores es muy fluctuante. 
- Las tres comunas con mayor cantidad de víctimas fatales son la 1, la 4 y la 9.

## KPIs

### KPI #1:

El objetivo a lograr era reducir en un 10% la tasa de homicidios en siniestros viales de los últimos seis meses, en CABA, en comparación con la tasa de homicidios en siniestros viales del semestre anterior.

En este sentido si se logró el cumplimiento de este KPI para el segundo semestre de 2021 pues se obtuvo una tasa de homicidios semestral de 1.354, es decir, es 23,63% menor que la tasa de homicidios semestral para el primer semestre de 2021, la cual fue de 1.773.

### KPI #2:

El objetivo a lograr era reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, en CABA, respecto al año anterior.

En este sentido No se logró el cumplimiento de este objetivo pues en comparación con el año 2020 se incrementó un 58.62% la cantidad de víctimas mortales de motocicletas para el año 2021. 

Es importante tener en cuenta que durante el año 2020 se produjo una reducción de accidentes debido al confinamiento por Covid-19, por lo que esto puede alterar los patrones de fallecimiento en accidentes.

## Conclusiones

- Se evidencia que las víctimas mortales de los siniestros viales suelen tener alguna de estas características: estar en un rango de edad de entre los 16 y los 45 años de edad, ser hombre, conducir moto o ser peaton. Por lo que las politicas de prevención y las estrategias de seguridad vial deben estar dirigidas a estos grupos demográficos.

- Al replantear y evaluar cualquier acción basada en estos análisis, es pertienente tomar en consideración el año 2020 como un año con algunos datos atípicos producto del confinamiento.

- 

 



