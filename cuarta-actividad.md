# Cuarta actividad: tu historia de periodismo de datos

![infografia](/img/delitos-mujeres.png "gráfico sobre los tipos de delitos cometidos por mujeres en 2020")

## Memoria

### INE

En primer lugar, he decidido modificar los datos y no seguir con los que utilicé para la actividad 3. Para ello, he acudido a la página del INE y he hecho una búsqueda para ver cuáles podían ser más acertados para este trabajo.

Como este cuatrimestre estoy haciendo los TFG, he aprovechado para realizar un gráfico que me pueda servir para insertarlo en mi reportaje escrito. Este versa sobre la situación de las mujeres en las cárceles de Madrid. Por ello, decidí coger los [resultados nacionales de condenados](https://www.ine.es/dynt3/inebase/es/index.htm?padre=4726&capsel=3978#), y, dentro de esto, los delitos según el sexo. 

Estos datos procedí a descargármelos en formato CSV, separado por ;.

### Open Refine

Cargué el fichero que me había descargado en la aplicación de Open Refine y procedí a hacer una limpieza y criba de datos.

En primer lugar, transformé la columna de los años en fecha, y usé el comando value.toString (‘yyyy’) para quedarme solo con los años. Tras esto, cribé los datos y me quedé solo con el último año, es decir, 2020, pues había datos desde 2013, gracias a la faceta de línea de tiempo.

Tras esto, procedí a la columna ‘sexo infractor’ para, con el filtro de texto, quedarme solo con los delitos cometidos por mujeres.

En la columna en la que se notifica el número de delitos, utilicé la transformación a número y la faceta numérica para descartar aquellos delitos que no se tuviera registros y su valor fuese 0.

Finalmente, en la columna en la que se tipifican los delitos, utilicé la función de faceta de texto. Con ello, pude cribar aún más los resultados pues me quedé solo con delitos generales y descarté los específicos. Por ejemplo, elegí la categoría ‘homicidios’ pero eliminé las subcategorías ‘homicidio’, ‘asesinato’ y ‘homicidio por imprudencia’.

Cuando los datos ya estaban listos, exporté el resultado final en CSV o ‘valores delimitados por comas’.

### Datawrapper

Cargué el archivo CSV que me había descargado con el anterior programa.

#### *Check & Describe*

Datawrapper detectó que la tercera columna correspondía a una fecha y que la última se trataba de números, pues es el total de delitos. El programa empleó el color verde y azul para identificarlas. De igual forma, se comprobó que ninguna celda aparecía en rojo, lo que indicaba que no había ningún problema con el archivo creado.

#### *Visualize*

En este paso se elige el tipo de gráfico deseado. En este caso, utilicé un gráfico de columnas horizontales pues como los nombres de los delitos son tan amplios si empleaba otro tipo de gráfico se solapaban estos. Así, con esta elección, es mucho más visual y facilita conocer cuáles son los delitos que más o menos cometieron las mujeres en 2020. Asimismo, he empleado el tono naranja pues, gracias a la cultura cinematográfica, se asocia este a la vestimenta típica de los centros penitenciarios. Además, es un color llamativo que llama a fijar la vista en los datos.

Después de esta elección, añadí el título y la breve descripción. En el pie de imagen, se incluye la autoría del gráfico (Azahara Serrano), la fuente de datos original (INE) con hipervínculo a la misma y la atribución de la herramienta. 

#### *Publish & Embed*

Tras publicar la infografía, Datawrapper ofrece descargar la imagen en formato .png, tal y como se ha adjuntado en este archivo. También permite compartirla a través de un enlace.

## Comentario del gráfico

Los datos que se han empleado para el gráfico son bastantes simples. Quizás habría estado interesante una comparativa con los delitos que cometen los hombres o una segmentación por nacionalidades.

Es acertado haberse quedado solo con el año 2020 pues, probablemente, los datos no varíen de forma muy significativa entre uno u otro año.

Por otro lado, se trata de un gráfico bastante tradicional en el que no hay una gran innovación. Sin embargo, a la hora de visualizar los datos, estos poseen un gran nivel de legibilidad y ayudan a su interpretación. No aparecen apilados ni los números ni las letras, lo cual es de agradecer.

Finalmente, el color empleado, también hace que sea llamativo, un tono más neutro o sobrio no habría beneficiado al gráfico.


