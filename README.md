# PRACTICA-ETL_PENTAHO
</h1> Este proyecto contiene un ejercicio integral de práctica con desafíos proporcionados por Chat GPT, desarrollado con Pentaho Data Integration (PDI). <br/> 
<h1>Enunciado de Ejercicio ETL con Pentaho: Base de Datos de Alumnos</h1>  </br>
Objetivo: Realizar un proceso ETL (Extracción, Transformación y Carga) para integrar y analizar los datos de los alumnos de la institución utilizando Pentaho Data Integration (PDI).</br>
<h2>Descripción del Problema:</h2>
En una base de datos histórica que contiene información sobre los alumnos de una institución educativa desde el año 2008 hasta el año 2023. Los datos incluyen detalles como el año de ingreso, género, grado, grupo, fecha de nacimiento, edad, nivel educativo, categoría, unidad académica, sede, programa educativo, nacionalidad, estado de nacimiento y si hablan una lengua indígena.</br>

<h3>Pasos del Proceso ETL:</h3>  
<h4>1.	Extracción:</h4>

- Cargar los datos desde el archivo CSV proporcionado.
 
<h4>2.	Transformación y carga:</h4></br>

o	Limpieza de datos:

- Eliminar filas duplicadas (las filas duplicadas saldrán de la cruza entre datos el GENERO, ESTADO DENACIMIENTO Y FECHA DE NACIMIENTO).
- Eliminar filas que en la fecha de nacimiento no respeten el formato DD/MM/YYYY
- Generar un archivo CSV con los datos eliminado y el motivo del error.
  
o	Generar 2 salidas en formato Excel </br>
- Primera salida:
     -  Calcular el número total de alumnos por año, 
     -  Calcular el número total por genero de cada año
     -  Calcular porcentaje de alumnos por género en cada año.</br>
- Segunda Salida:
     -  Generar una campo llamado FECHA_INSCRIPCION el cual deberá tener como fecha 01/01/ AÑO ( El año deberá ser tomado del campo AÑO)
     -  Calcular la edad de los alumnos en función de su fecha de nacimiento y la fecha de inscripción antes solicitada.
     -  Calcular la edad de los alumnos en función de su fecha de nacimiento y la fecha actual.
     -  En el archivo solo se requiere información de los inscriptos que tienen menos de 40 años y el nivel educativo es PREPARATORIA </br>
<h3>  Requisitos del Proyecto:</h3>  
•	Crear un Job en Pentaho Data Integration que contenga todos los pasos de Extracción, Transformación y Carga.


<h3>Curso de YouTube</h3>
El curso en el cual se basan estas transformaciones se puede encontrar en la siguiente URL:

- [Curso de ETL con Pentaho](https://www.youtube.com/playlist?list=PLPgjON4ZM0JBdxxDUAfCS84X79e_2CLNQ)

<h3>Documentación de Ayuda</h3>
Para mayor información y ayuda sobre el uso de Pentaho, se consulto las siguientes documentaciones:

- [Documentación Pública de Pentaho](https://docs.hitachivantara.com/r/en-us/pentaho-data-integration-and-analytics/9.3.x/mk-95pdia003/pdi-transformation-steps)
- [Pasos de Transformación de PDI](https://pentaho-public.atlassian.net/wiki/spaces/EAI)

