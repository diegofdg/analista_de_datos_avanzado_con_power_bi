# Preguntas
1) ¿Cuál fue el mes con la mayor cantidad de ventas en unidades de productos? ¿Y cuál fue el mes con la menor cantidad?
2) ¿Cuál fue el mes con la mayor facturación? ¿Y el de menor facturación?
3) ¿Cuáles son los 3 productos con la mayor cantidad de unidades vendidas durante todo el periodo?
4) En el mes de julio, ¿cuántas unidades de auriculares inalámbricos se vendieron? ¿Qué porcentaje representan del total de unidades vendidas de todos los productos en ese mes?
5) ¿Cómo estuvieron compuestas las ventas de productos de belleza y cuidado personal en el mes de julio? ¿Y en todo el periodo analizado?
6) ¿Qué tendencia muestra la facturación de los productos de "Hogar y jardín" durante todo el periodo analizado?

# Pasos para la solución del proyecto del día 1
1) Descarga los datos de la lección "Proyecto del Día 1" y cárgalos en tu archivo de Power BI a través de Inicio / Datos / Obtener Datos / Texto o CSV
2) En la ventana de Power Query, asegúrate de que los datos se ven bien, modifica algo si es necesario, y luego haz click en "Cargar".
3) En la vista de tabla puedes modificar el formato de algunos campos, si lo deseas.
4) Observa que la pregunta 1 contiene 2 elementos en su formulación: "Mes" (esta información corresponde al campo Fecha) y "Ventas de unidades" (esta información corresponde al campo Cantidad de unidades).   
Elije un gráfico que te permita ver el comportamiento de las cantidades de unidades a lo largo del tiempo. Yo he elegido Gráfico de Líneas, pero no es la única opción. Ten presente que las fechas contienen muchas categorías (Año, Trimestre, Mes y Día), por lo que es probable que debas descender en las jerarquías hasta poder visualizar los meses.
5) Observa que la pregunta 2 es muy similar a la anterior, ya que también evalúa el comportamiento de un atributo a lo largo del tiempo, pero esta vez está relacionado al dinero. Puedes generar un nuevo gráfico copiando y pegando el gráfico anterior, y luego cambiando Cantidad de unidades por Monto Total.
6) La pregunta 3 solo pide evaluar una variable, que es la cantidad de unidades. Elije un gráfico que acumule esas cantidades y las ordene de mayor a menor. Yo utilicé un gráfico circular, pero esa no es la única opción.
7) La pregunta 4 puede ser respondida con el gráfico anterior, ya que podemos ver ese producto tanto en sus cantidades como en su porcentaje. El problema es que nuestro gráfico actual representa a todo el período de tiempo, mientras que esta pregunta pide los datos de Julio. Entonces debemos filtrar los datos mostrados. Hay varias formas de hacer esto. Una de ellas podría ser agregar un segmentador a nuestro gráfico, que filtre el campo Fecha, y luego establecer que el período de tiempo mostrado sea desde el 01 hasta el 31 de Julio.
8) La pregunta 5 nos vuelve a pedir datos segmentados en el mes de Julio, por lo tanto nuestro segmentador sigue siendo útil tal como está. Por otro lado nuestro actual gráfico de productos nos va a servir para visualizar la información que necesitamos. Lo único que necesitamos agregar es un nuevo segmentador para el campo Categoría, de modo que el gráfico solo muestre los productos de Belleza y Cuidado personal.
9) La pregunta 6 solo nos pide identificar, a través del tiempo, si la facturación de los productos de esa categoría aumentó, se mantuvo estable, o disminuyó. Para responder a esta pregunta no debemos agregar ningún gráfico ni segmentador. Solo debemos ajustar el segmentador de Categoría para que muestre los productos que nos interesan, asegurarnos de que el segmentador de Fecha muestre todo el período, y luego mirar el gráfico de Monto, para identificar la tendencia solicitada.

# Respuestas
1) Mayor: Mayo / Menor: Septiembre
2) Mayor: Mayo / Menor: Junio
3) Bicicleta de montaña // Gafas de sol // Telefono inteligente
4) Cantidad: 52 // Porcentaje: 13,16%
5) En Julio: Perfume de mujer: 56% // Crema hidratante facial: 44%  
   En Todo el período: Secador de Cabello: 32,23% // Perfume para mujer: 24,91 // Crema hidratante facial: 24,18% //Paleta de sombras de ojos: 16,48% // Cepillo de dientes eléctrico: 2,2%
6) Decreciente
