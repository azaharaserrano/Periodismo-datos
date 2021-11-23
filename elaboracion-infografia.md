# Infografía con los datos del proyecto TRESCA

## Gráfico de elaboración propia

![infografia](/img/infografia-tweets.png "gráfico sobre los tweets que incluían un hashtags de Feliz Navidad")

Se ha utilizado el proyecto TRESCA para extraer sus datos y crear el gráfico de líneas que se puede observar. En el eje X u horizontal se han representado los valores de fecha (desde octubre hasta diciembre), mientras que, en el Y o vertical, la variable 'número de tweets'.

Se debe recalcar que solo se han utilizado los hashtags de ‘#FelizNavidad’ con más de 10.000 tweets, puesto que se parte de dicha cifra a la hora de contabilizarlos. Por tanto, en el gráfico se muestran los tweets que se han publicado con el hashtag mencionado desde principios de octubre hasta el día de Navidad. Con ello podemos saber desde cuándo se comienza a hablar de esta festividad y, si tuviéramos datos de años anteriores, podríamos saber si la tendencia a hablar antes de ella aumenta o disminuye con el tiempo.

Por otro lado, se ha recurrido a usar un tono rojo oscuro pues es el color que suele destacar en estas fechas señaladas.

## Memoria 

### Open Refine

Para tratar el archivo feliz.csv se ha recurrido a utilizar el programa Open Refine. En primer lugar, he eliminado varias columnas cuya información no era relevante para el trabajo, por ejemplo, en la que aparece el hipervínculo del tweet en concreto. Para poder trabajar con estos datos, eliminé varias columnas cuya información no era relevante para la infografía planteada.  Tras esta limpieza, el resultado fue el de contar con tres columnas: fecha, hashtag y número de tweets.

Tras esto, he utilizado opción de 'transformaciones comunes' para dar formato de fecha a la primera columna y de número a la última. Este paso es necesario si se quiere trabajar con las facetas, que permiten segmentar los datos con facilidad.

Agrupé los hashtags que eran similares para acotar más las filas, por ejemplo, si uno era ‘Feliz Sabado’ y otro ‘Feliz Sábado’.

Utilicé la función de faceta numérica para que se mostraran solo hashtags que tuviesen un valor en la columna de número de tweets. Por tanto, se filtraron los que no tenían una celda en blanco en esta columna.

Asimismo, filtré la columna de hashtags para quedarme solo con los que hablaran de Navidad.

Después de estos pasos, recurrí a tratar la columna de las fechas pues no me eran relevantes saber las horas, simplemente quería quedarme con los días y meses. Para ello, las transformé con la función ‘value. toString(‘yyyy-MM-dd’)’.

Finalmente, exporté el proyecto en formato .csv (comma separated values o valores separados por comas) para poder abrirlo con Datawrapper.

### Datawrapper

Cargué el .csv en este programa.

#### Check & Describe

Datawrapper detectó que la primera columna de datos correspondía a una fecha y lo mismo ocurrió con la columna de cantidad de tweets. El programa empleó el color verde y azul para identificar las mismas. De igual forma, se comprobó que ninguna celda aparecía en rojo, lo que indicaba que no había ningún problema.

#### Visualize

En este paso se elige el tipo de gráfico deseado. Me centré en un gráfico de líneas puesto que permite ver de una forma más visual una evolución temporal, lo cual era el objetivo a conseguir.

Además, añadí el título, la breve descripción y footer o pie de imagen. En este se incluye la autoría del gráfico (Azahara Serrano), la fuente de datos original (proyecto TRESCA) y la atribución de la herramienta. También incluye la anotación sobre la consideración de los datos que fueran iguales o superiores a los 10.000 tweets.

#### Publish & Embed

Tras publicar la infografía, Datawrapper ofrece descargar la imagen en formato .png, tal y como se ha adjuntado en este archivo. También permite compartirla a través de un enlace. 

