# Consigna para el Proyecto del Día 11
Llegó la hora de poner a prueba una vez más nuestros conocimientos, y hoy tenemos un desafío muy interesante por delante. Vas a recibir los datos del producto bruto interno de varios países (expresados en su moneda nacional) y también información sobre su población. Antes que nada es importante aclarar que esta información es ficticia y que fue desarrollada solo a fines pedagógicos.  
Lo que tu deberás hacer es calcular el PBI per cápita (es decir, el Producto Bruto Interno por habitante). Este valor tiene que estar expresado en dólares estadounidenses (a fines de que sean valores comparables entre países), y luego debes mostrarlo en un gráfico de dispersión, donde un eje sea la población, el otro el PBI per cápita calculado, y cada punto represente a un país. El tamaño de esos puntos debe ser proporcional a su PBI en millones de dólares estadounidenses.  
De más está decir que deberás recurrir a DAX y al modelo de datos para crear las relaciones necesarias entre las tablas, y calcular los datos que necesitas para llegar a la visualización de la consigna. Una vez hecho eso, vas a tener que responder un par de preguntas para comprobar si tus resultados son correctos.  

# Preguntas
1) ¿Cuáles son los dos países que se apartan más del resto en el gráfico de dispersión?
2) ¿Cuáles son los dos países que se destacan por el tamaño de su burbuja en la visualización?
3) ¿Cuál es el PBI por habitante calculado en USD para el país que se encuentra en Oceanía?

# Pasos para la solución del proyecto del día 11
1) Importa las dos tablas de Excel que encontrarás en el archivo que descargaste en la lección anterior.
2) Crea una medida donde se calcule el valor en dólares estadounidenses del PBI de cada país. Para hacerlo debes dividir el PBI por tipo de cambio. Esto va a implicar que vincules o combines las tablas de alguna manera (ya sea en el modelo de datos, o en la ventana de Power Query).  
Alternativa:  puedes hacerlo sin vincular o combinar las tablas, usando una función de DAX llamada RELATED. Si quieres hacerlo de esta manera, investiga en internet cómo funciona RELATED. De lo contrario, procede con los métodos que ya conoces.
3) El siguiente paso, es crear una nueva medida donde esté calculado el PBI per cápita (por habitante) de cada país. Por lo tanto debes dividir el PBI (en dólares) de cada país, por la población de cada país.
4) Con ambas medidas claculadas, ya estás en condiciones de crear el gráfico de dispersión que te permitirá visualizar el PBI per cápita de cada país. No olvides asociar el tamaño de cada círculo con el valor del PBI para poder identificar fácilmente las respuestas.  
Para resolver la pregunta sobre un país de Oceanía, puede que agregar algún segmentador o filtro te facilite las cosas aún más.

# Respuestas
1) India y China
2) EEUU y China
3) 50,76