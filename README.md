# Análisis De Siniestros Viales en la Ciudad De Buenos Aires, Argentina
Realizado por: Cristian Silva

En este proyecto, se busca realizar un análisis exhaustivo de los datos relacionados con los siniestros viales ocurridos en la Ciudad de Buenos Aires entre los años 2016 y 2021. El propósito principal es proporcionar a las autoridades locales información detallada y precisa que les permita tomar medidas concretas para reducir el número de víctimas fatales causadas por estos incidentes.

## Indice

 - [Contexto](#Contexto:)
 - [Tecnologías utilizadas](#Tecnologías utilizadas)
 - [Estructura del repositorio](#Estructura del repositorio)
     - [Notebooks](###Notebooks)
     - [Data](###Data)
     - [KPIS](###KPIS)
 - [Proceso de trabajo](##Proceso de trabajo)
     - [ETL y EDA](###ETL y EDA)
     - [Análisis de los datos](###Análisis de los datos)
 - [KPI's](##KPI's)
     - [KPI 1: Métrica de Seguridad en Accidentes Vehiculares](##)
     - [KPI 2: Incidentes Mortales Involucrando Motociclistas](##)
     - [KPI 3: Enfoque en el Mayor Responsable de Siniestros Viales del Último Semestre](##)
 - Reflexiones](##)
     - [Contextualización de Datos Temporales](##)
     - [Roles y Edades de las Víctimas](##)

 - [Sugerencias](##)
     - [Monitoreo Activo en Diciembre](##)
     - [Participación Comunitaria Continua](##)
     - [Análisis Continuo de Datos](##)

## Contexto:

Los siniestros viales se definen como cualquier evento o incidente que ocurre en las vías públicas e involucra vehículos de motor, peatones o ciclistas, resultando en daños materiales, lesiones o pérdida de vidas humanas. Este fenómeno ha llevado a diversas regiones a mantener registros detallados de las tasas de mortalidad asociadas con los siniestros viales, con el objetivo de reducir dichas cifras mediante la implementación de medidas que abarcan desde la educación vial, hasta la mejora de la infraestructura y la promoción de vehículos seguros.

En el caso particular de la ciudad de Buenos Aires, emerge una preocupación significativa frente a este tipo de sucesos, dado su carácter de metrópolis con un tráfico intenso y una alta densidad poblacional. Según revela el Sistema Nacional de Información Criminal (SNIC), entre los años 2018 y 2022 se contabilizaron 19,630 muertes a causa de siniestros viales, lo que representa un promedio de 11 personas fallecidas diariamente en tales circunstancias. Estos incidentes no solo implican un riesgo para la seguridad de los habitantes de la ciudad, sino que también afectan la infraestructura urbana y la capacidad de los servicios de emergencia para responder eficazmente.

Por tanto, la importancia de un proyecto de esta envergadura radica en su capacidad para no solo llevar un seguimiento detallado de las estadísticas, sino también para evaluar y poner en práctica políticas destinadas a mitigar este problema de manera efectiva.

## Tecnologías utilizadas
Para el desarrollo de este proyecto se utilizaron las siguientes tecnologías: Phyton 3.10, Pandas, NumPy, Warnings, GeoPy, matplotlib, seaborn y spicy. 
 
## Estructura del Repositorio
- Data:
   - `c2022_caba_est_c1.xlsx`: Datos estadísticos de la población de CABA.
   - `homicidios_hechos.csv`: Información sobre los hechos de siniestros viales.
   - `homicidios_victimas.csv`: Datos sobre las víctimas de siniestros viales.
- Notebooks:
   - `EDA.ipynb`: Jupyter Notebooks del análisis Exploratorio de Datos de los siniestros viales.).
   - `ETL.ipynb`: Jupyter Notebooks del proceso de Extracción, Transformación y Carga de los datos de siniestros viales.
      
- KPIs: Archivos CSV con los indicadores clave de rendimiento para evaluar los siniestros viales.
    - `kpi1.csv`: Reducir en un 10% la tasa de homicidios en siniestros viales de los últimos seis meses, en CABA, en comparación con la tasa de homicidios en siniestros viales del semestre anterior.
    - `kpi2.csv`: Reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, en CABA, respecto al año anterior.
    - `kpi3.csv`: Reducir en un 5% el número de accidentes mortales en el ultimo semestre en CABA, ocasionados por el mayor responsable de siniestros viales del ultimo semestre, respecto al mismo responsable en el semestre anterior.
- `README.md`: Descripción general del proyecto.
 accidentes de tráfico. Se entregará un informe detallado de las tareas realizadas, las metodologías adoptadas y las conclusiones clave. Además, se creará un dashboard interactivo para facilitar la interpretación de los datos y su análisis.

## Proceso de trabajo

### ETL y EDA
Se realizó un proceso ETL en el cual se realizó una visualización inicial, estandarizar variables, limpieza de datos mediante el analisis y eliminación de nulos, revisión y eliminación de duplicados y columnas redundantes. Posteriormente, se llevó a cabo un análisis exploratorio para identificar patrones y tendencias que ayuden a tomar medidas preventivas.

### Análisis de los Datos
El análisis integral de los datos sobre siniestros viales en la Ciudad Autónoma de Buenos Aires (CABA) revela patrones y tendencias significativas:

#### Datos Generales:
- El conjunto de datos cuenta con 707 registros y 25 columnas, proporcionando información detallada sobre accidentes, víctimas, ubicación y detalles temporales.

#### Características Temporales:
- Los accidentes parecen distribuirse de manera relativamente uniforme a lo largo de los años, meses y días, con un promedio de 1.06 víctimas por incidente.
- Analizando cada año en particular, el 2020 fue un año donde disminuyó mucho la tasa de siniestros viales, esto puede ser consecuencia de la cuarentena impuesta por las autoridades en base a la pandemia de COVID-19.

#### Ubicación y Franja Horaria:
- La mayoría de los accidentes ocurren en las franjas horarias de 6:00 a 12:00 y de 18:00 a 24:00 horas, y la Comuna 1 es la más afectada.
- Las avenidas son escenarios comunes de accidentes, representando el 62% de las víctimas, con un pico los sábados.

#### Edad:
- La edad promedio de las víctimas es de aproximadamente 42 años.
- La edad promedio de las victimas mujeres es de 53 años y de hombres es de 40 años
- La mayoría de las víctimas tienen edades comprendidas entre 20 y 40 años, destacando la importancia de dirigir estrategias de seguridad vial a este grupo.

#### Género:
- El 76.6% de las víctimas son masculinas, siendo este género predominante en todos los roles, ya sea conductor, pasajero o peatón.

#### Roles y Responsabilidad:
- El 48% de las víctimas desempeñaba el rol de conductor, principalmente en motos.
- Los conductores de automóviles, colectivos y camiones son responsables en el 75% de los casos donde se señala un vehículo como responsable.

#### Distribución Espacial:
- La alta frecuencia de accidentes en avenidas en la mayoría de las comunas de la Ciudad Autónoma de Buenos Aires indica posibles áreas críticas con alto flujo vehicular y, por ende, mayores riesgos de siniestros viales.

#### Patrones Temporales:
- Se observa un aumento en la cantidad de accidentes en diciembre.
- Los picos de accidentes en diferentes meses varían en distintos años. Aunque se puede observar un patrón anual en la distribución de incidentes, destacando un pico significativo en diciembre, este mes experimentó la mayor cantidad de incidentes. Contrastando con esta tendencia, abril surge como el mes con la menor cantidad de incidentes registrados. Este análisis revela una tendencia general de disminución gradual de incidentes desde enero hasta abril, seguida de un aumento constante en los meses de mayo, junio, agosto y noviembre.

#### Relación entre Víctimas y Acusados:
- Las motos son frecuentes víctimas pero raramente acusadas. Los autos, por otro lado, son comunes en ambos roles.

Este análisis integral proporciona una visión completa de la problemática de los siniestros viales en la Ciudad Autónoma de Buenos Aires.

## KPI (Indicadores Clave de Rendimiento)
En el marco del análisis de los siniestros viales y con el objetivo de reducir la cantidad de víctimas fatales, se han definido dos Indicadores Clave de Rendimiento (KPI) que abordan aspectos específicos de la seguridad vial en CABA. Para poder realizar el análisis de los indicadores se crearon Tablas para facilitar dicho proceso.

### KPI 1 - Métrica de Seguridad en Accidentes Vehiculares:
La métrica de seguridad en accidentes vehiculares se configura como un indicador esencial, evaluando el número de víctimas fatales en incidentes de tráfico por cada 100,000 habitantes durante un semestre. La meta consiste en reducir esta métrica en un 10% en el segundo semestre de 2021 en comparación con el primer semestre. El análisis demuestra que al alcanzar una métrica de 1.35, se superó con éxito el objetivo de disminuir en un 10% la tasa de fatalidades, ya que la métrica previa era de 1.73, logrando así una reducción del 22.22%.

### KPI 2 - Incidentes Mortales Involucrando Motociclistas:
El segundo KPI se encarga de supervisar la cantidad de incidentes mortales relacionados con motociclistas. El propósito es reducir en un 7% la cantidad de accidentes mortales de motociclistas durante el último año. No obstante, los resultados indican un aumento del 79.21% en la cifra de fallecimientos de motociclistas en 2021, señalando la necesidad de estrategias adicionales. Es importante tener en cuenta que el año 2020 estuvo marcado por una pandemia y restricciones de movimiento, lo cual impactó la circulación en las calles.

### KPI 3 -  Enfoque en el Mayor Responsable de Siniestros Viales del Último Semestre:
El segundo KPI se encarga de supervisar la cantidad de incidentes mortales relacionados con motociclistas. El propósito es reducir en un 7% la cantidad de accidentes mortales de motociclistas durante el último año. No obstante, los resultados indican un aumento del 79.21% en la cifra de fallecimientos de motociclistas en 2021, señalando la necesidad de estrategias adicionales. Es importante tener en cuenta que el año 2020 estuvo marcado por una pandemia y restricciones de movimiento, lo cual impactó la circulación en las calles.

En resumen, es menester ajustar las estrategias existentes y desarrollar nuevas iniciativas para hacer frente a los desafíos identificados por los KPI.

## Reflexiones
### Contextualización de Datos Temporales:
La observación detallada de los datos revela que el año 2020 presenta una disminución significativa en la tasa de siniestros viales, atribuible a las restricciones implementadas durante la cuarentena por la pandemia de COVID-19.

### Roles y Edades de las Víctimas
El grupo de edad entre 20 y 40 años es particularmente vulnerable. Es esencial dirigir las estrategias de seguridad vial específicamente a este segmento de la población para lograr un impacto significativo.

## Sugerencias
### Monitoreo Activo en Diciembre:
Dada la tendencia anual de aumento en diciembre, intensificar las medidas de seguridad y aplicación de la ley durante este mes.

### Participación Comunitaria Continua:
Establecer canales de retroalimentación y colaboración puede fortalecer las iniciativas de seguridad vial.

### Análisis Continuo de Datos:
Establecer un sistema de análisis continuo de datos para detectar patrones emergentes y ajustar estrategias según la evolución de la situación.


