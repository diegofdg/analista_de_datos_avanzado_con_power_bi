# Consigna para el Proyecto del Día 12
¡Felicidades por llegar hasta aquí!  Un nuevo día más que se acaba, y nada mejor en mi opinión que un buen desafío para terminar de asentar este torbellino de nuevos conocimientos que has adquirido. Así que prepárate y presta mucha atención a las indicaciones (ya que serán bastante precisas) para que puedas llevarlas a cabo.  
Te propongo el siguiente desafío: descarga el cuerpo de datos que viene junto a esta lección, y utiliza tus nuevos conocimientos de DAX para calcular, para cada país, qué porcentaje de ventas de más de una unidad se realizan sobre el total de ventas que ese país tiene. Si por ejemplo, Colombia hubiera realizado 4 ventas en el periodo, y solo una de ellas hubiera sido de más de una unidad vendida (este dato se encuentra en el campo Cantidad), mientras que todas las demás ventas fueron de solamente una unidad, entonces el valor para Colombia sería de 25% (en otras palabras, esto quiere decir que el 25% de las ventas de Colombia son por más de una unidad).  
Luego, calcula cómo ha cambiado ese porcentaje entre 2024 y 2025 para cada país, y muestra todos estos resultados en una matriz. Nada más, ni nada menos, que eso.  
Recuerda emplear medidas, cuando lo necesites ayúdate con medidas rápidas y con la función CALCULATE, y finalmente optimiza tu expresión empleando variables.  
Al finalizar, responde a las preguntas del proyecto de hoy.

# Preguntas
1) ¿La cantidad global de ventas de más de una unidad, para todos los países en su conjunto, ha aumentado o disminuido entre 2024 y 2025? ¿Cuál fue la variación porcentual entre ambos años?
2) Para el país que mayor proporción de ventas no unitarias realiza, ¿cuál fue su variación interanual entre 2024 y 2025?
3) ¿Cuál fue el país que más vio disminuir su proporción de ventas no unitarias entre 2024 y 2025?

# Pasos para la solución del proyecto del día 12
1) Importa los datos a tu modelo.
2) Crea una matriz en la que colocarás los países como filas.
3) Escribe una medida que calcule el porcentaje de ventas mayores a una unidad (ventas no unitarias).  
Tip 1: este porcentaje sería, básicamente, una división entre la cantidad de ventas mayores a una unidad, y la cantidad de ventas totales.  
Tip 2: Si bien la operación es simple (una división), construir los valores que van a intervenir en esta operación puede ser un desafío. Te recomiendo usar variables para visualizar mejor los componentes de tu medida, y acudir a funciones como CALCULATE o COUNTROWS para alcanzar los valores que necesitas identificar.
4) Agrega a tu matriz la medida que has creado, e identifica qué campo deberías incorporar a esta visualización para poder ver los valores distribuidos en los años que abarca el modelo de datos.
5) Ahora debes crear una medida que te permita identificar la variación interanual, es decir, en qué porcentaje disminuyó o aumentó la cantidad de ventas no unitarias entre año y año.  
Esto puede ser algo complejo, por lo que si no puedes escribirlo por tí mismo, te recomiendo hacerlo con las medidas rápidas ¿Hay alguna que permita establecer variaciones año a año?
6) Agrega esta última medida a tu modelo de datos, para poder ver esa variación numéricamente, y país por país, para que puedas responder a las preguntas del siguiente cuestionario.

# Respuestas
1) Disminuyó un 4,01%
2) 0%
3) Colombia