#### Proyecto Individual 2: Data Analyst. Henry, Data Science Full Time 22, Franco D'Auro.

##### Introducción

En este repositorio se presentan los archivos de un proyecto en el que se simula el desempeño de un Data Analyst. Particularme se pretende asistir al Observatorio de Movilidad y Seguridad Vial (OMSV), dependiente de la Secretaría de Transporte del Gobierno de la Ciudad Autónoma de Buenos Aires Ciudad. Esta organización pretende disminuir los accidentes fatales que ocurren en la Ciudad Autónoma de Buenos Aires (CABA). Para ello, el OMSV ha facilitado un dataset con valiosos datos sobre los accidentes viales ocurridos en CABA y sobre las víctimas afectadas. Por lo tanto se procede a analizar el dataset provisto para generar la información necesaria que permita asistir la toma de desiciones del OMSV.

##### Materiales y métodos

El dataset provisto consta de dos archivos llamados 'homicidios.xlsx' y 'Diccionario de datos Siniestros viales.xlsx'. El archivo 'homicidios.xlsx' tiene dos páginas, una llamada 'HECHOS' con datos relacionados a los accidentes viales, mientras que la otra se denomina 'VICTIMAS' y aporta información sobre las personas afectadas. En el archivo 'Diccionario de datos Siniestros viales.xlsx' se encuentran el significado real de las variables asociadas tanto a los accidentes, como sus víctimas.
Los datos presentes en 'homicidios.xlsx' se sometieron a un Análisis Exploratorio de Datos (EDA por sus acrónimo en inglés) en el que se llevaron a cabo las siguientes tareas:
1. Seleccion de los campos (columnas) útiles y sin redundancias.
2. Corrección de nombres de campos.
3. Búsqueda y codificación de valores faltantes.
4. Eliminacion de registros (filas) vacías.
5. Identificar y corregir el tipo de datos por campo.
6. Búsqueda y eliminación de registros repetidos.
7. Verificación de la correcta estructura de cada tabla de datos realizada.
8. Búsqueda de valores atípicos/extremos u outliers de las variables cuantitativas.
9. Gráficos descriptivos coherentes según la tipología de variable.
10. Documentación de las primeras conclusiones.

Con los datos limpios generados en el EDA se crearon dos archivos de texto plano llamados 'HECHOS.csv' y 'VICTIMAS.csv'. El archivo 'HECHOS.csv' porta datos sobre los accidentes viales, mientras que 'VICTIMAS.csv' describe la situación de las personas afectadas. Estos archivos se utilizaron para realizar visualizaciones en tableros de control interactivos (dashboard) para obtener conclusiones útililes para la toma de desiciones.
A continuación se nombran las visualizaciones realizadas:
1- Gráficos de línea.
2- Filtros interactivos.
3- Tarjetas con medidas propias.
4- Gráficos de barras simples y apiladas
5- Histogramas
6- Mapa con puntos georreferenciados

