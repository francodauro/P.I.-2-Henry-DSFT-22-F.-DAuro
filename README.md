#### Proyecto Individual 2: Data Analyst. Henry, Data Science Full Time 22, Franco D'Auro.

##### Introducción

En este repositorio se presentan los archivos de un proyecto en el que se simula el desempeño de un Data Analyst. Particularme se pretende asistir al Observatorio de Movilidad y Seguridad Vial (OMSV), dependiente de la Secretaría de Transporte del Gobierno de la Ciudad Autónoma de Buenos Aires. Esta organización pretende disminuir los accidentes fatales que ocurren en la Ciudad Autónoma de Buenos Aires (CABA). Para ello, el OMSV ha facilitado un dataset con valiosos datos sobre los accidentes viales ocurridos en CABA y sobre las víctimas afectadas. Por lo tanto se procede a analizar el dataset provisto para generar la información necesaria que permita asistir la toma de desiciones del OMSV.

##### Materiales y métodos

El dataset provisto consta de dos archivos llamados 'homicidios.xlsx' y 'Diccionario de datos Siniestros viales.xlsx'. El archivo 'homicidios.xlsx' tiene dos páginas, una llamada 'HECHOS' con datos relacionados a los accidentes viales, mientras que la otra se denomina 'VICTIMAS' y aporta información sobre las personas afectadas. En el archivo 'Diccionario de datos Siniestros viales.xlsx' se encuentran el significado real de las variables asociadas tanto a los accidentes, como sus víctimas.
Los datos presentes en 'homicidios.xlsx' se sometieron a un Análisis Exploratorio de Datos (EDA por sus acrónimo en inglés) en el que se llevaron a cabo las siguientes tareas:
1. Selección de los campos (columnas) útiles y sin redundancias.
2. Corrección de nombres de campos.
3. Búsqueda y codificación de valores faltantes.
4. Eliminacion de registros (filas) vacías.
5. Identificación y corrección del tipo de dato por campo.
6. Búsqueda y eliminación de registros repetidos.
7. Verificación de la correcta estructura de cada tabla de datos depurada.
8. Búsqueda de valores atípicos/extremos u outliers de las variables cuantitativas.
9. Realización de gráficos descriptivos coherentes según la tipología de cada variable (cuantitativa o cualitativa).
10. Documentación de las primeras conclusiones.

Con los datos limpios generados en el EDA se crearon dos archivos de texto plano llamados 'HECHOS.csv' y 'VICTIMAS.csv'. El archivo 'HECHOS.csv' porta datos sobre los accidentes viales, mientras que 'VICTIMAS.csv' describe la situación de las personas afectadas. Estos archivos se utilizaron para realizar visualizaciones en tableros de control interactivos (dashboard) para obtener conclusiones útiles para la toma de desiciones.
A continuación se nombran las visualizaciones realizadas:
1. Gráficos de línea.
2. Filtros interactivos.
3. Tarjetas con medidas propias.
4. Gráficos de barras simples y apiladas
5. Histogramas
6. Mapa con puntos georreferenciados

Entre las medidas calculadas, tres de ellas se utilizaron como KPI (Key Performance Indicator: Indicador Clave de Rendimiento). Los KPI son medidas cuantitativas (métricas) de gran importancia que se contrastan con un valor de referencia asociado con una expectativa de logro. A continuación se presentan los tres KPI abordados:

* Tasa de Homicidios en Siniestros Viales = número de víctimas fatales en accidentes de tránsito por cada 100,000 habitantes en un área geográfica durante seis meses. Su fórmula es:
  
_Tasa de homicidios en siniestros viales = (Número de víctimas fatales / Población Total) * 100000_

La meta es reducir un 10 % la tasa de homicidios en el último semestre respecto del semestre anterior.

* Número de accidentes mortales de motociclistas en siniestros viales durante un año. Se pretende reducir un 7% el número de victimas fatales en moto durante el último año respecto del año anterior.

 * Número de accidentes mortales de peatones en siniestros viales durante un año. Se pretende reducir un 10% el número de victimas fatales de peatones durante el último año respecto del año anterior.

El EDA fue realizado en lenguaje Python 3 e interpretado por el entorno de desarrolo integrado Visual Studio Code (VSC) de Microsoft. Para mayor comodidad el código fue organizado en cuadernos (Notebook) utilizando la extensión de VSC llamada Jupyter. El dashboard fue realizado con la herramienta de visualización y análisis de datos Power BI de Microsoft.

##### Resultados

En el EDA se hicieron dos grandes grupos de gráficos: 1- histogramas de variables cuantitativas y, 2- gráficos de barras con el conteo de elementos de variables cualitativas.
Del análisis de los histogramas se pudieron realizar las siguientes observaciones preliminares:
1. El número de víctimas por año a decaído con el paso del tiempo.
2. El número de víctimas por día es constante a los largo del mes.
3. Durante fin de año se concentran los accidentes.
4. La mañana y la medianoche son los horarios con mayor riesgo de accidente.
5. El número de víctimas por accidente es generalmente igual a 1.
6. Los adultos jóvenes son los más accidentados.

Los gráficos de barras de las variables cualitativas sugieren lo siguiente:
1. La gran mayoría de los accidentes ocurren en avenidas y calles.
2. Los accidentes se concentran en el Sur y en el área comercial y turística (Ver Mapa de comunas de CABA).
3. La gran mayoría de las víctimas son peatones, o pasajeros de autos y motos.
4. La gran mayoría de las víctimas son hombres.
5. La gran mayoría de las víctimas con vehículo son conductores.
6. La mayoría de los acusados son pasajeros de autos y transporte de cargas.

El dashboard construido en Power BI corroboró las observaciones que resultaron de los gráficos del EDA. 

Los cambios observados en los KPI permitieron contrastar las metas buscadas tal como se detalla a continuación:
1. La Tasa de Homicidios en Siniestros Viales cayó un 12.5% durante los últimos 6 meses respecto al semestre anterior. Se cumplió con la meta de reducir un 10% esta tasa. 
2. El número anual de accidentes mortales de motociclistas aumentó un 58.62% respecto del año anterior. No se logró con la expectativa de reducir este número en un 7%. 
3. El número anual de accidentes mortales de peatones disminuyó un 5.71%% respecto del año anterior. No se logró con la expectativa de reducir este número en un 10%. 

##### Recomendaciones

En función de todos los resultados obtenidos. Se enuncian las siguientes sujerencias:

1. Realizar campañas de concientización y prevención vial sobre la población con las siguientes características: varones, menores de 50 años, peatones o conductores de moto, auto o vehículo de carga.
2. Reforzar los controles viales en avenidas y calles de las comunas 1, 3, 4 y 7, entre las 5 y 10 de la mañana.
3. Reforzar los controles viales durante Noviembre y Diciembre.
4. Se enfatiza la importancia de la prevención sobre la población de motociclistas ya que presenta un fuerte aumento en el riesgo de muerte por accidente. 

