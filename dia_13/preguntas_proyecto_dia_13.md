# Consigna para el Proyecto del Día 13
Ahora que hemos conocido y explorado las herramientas de inteligencia de tiempo, estoy seguro de que te sientes mucho más cómodo utilizándolas. ¡Por lo tanto es hora de poner ese conocimiento a prueba en el proyecto del día de hoy! En el desafío de hoy, vamos a incorporar la dimensión del tiempo para obtener una visión más completa de la salud financiera de nuestro negocio ficticio.  
Imagina que nuestra empresa cierra su balance el 30 de junio de cada año, lo que significa que su año fiscal comienza el 1 de julio. Usando las herramientas de inteligencia de tiempo, queremos analizar cómo ha sido el rendimiento en términos de generación de beneficios acumulados mes a mes durante el último año fiscal en comparación con el año anterior. Este análisis nos va a ayudar a tomar decisiones informadas y, si es necesario, a realizar correcciones.  
También, te desafío a mostrar esta variación en los beneficios a través de una visualización adecuada, que esté segmentada por categorías de productos. Esto nos va a permitir identificar qué categorías han tenido un mejor desempeño y cuáles han empeorado su rendimiento en el último año.  
Por otro lado no dejes de aplicar un formato condicional sobre esa visualización para hacerla dinámica y claramente interpretable.

# Preguntas
1) ¿Cuál de estas categorías de productos han mostrado una tendencia contraria a la general en términos de generación de beneficios, al comparar los beneficios acumulados en el año fiscal iniciado el 1/7/25?  
  a) Tarjetas de regalo  
  b) TV y Sonido  
  c) Cámaras  
  d) Electrónica para automóviles y GPS

2. ¿Cuál de las siguientes expresiones es correcta, al comparar los beneficios acumulados, en comparación con los del año anterior, cuando nos concentramos en  el año fiscal iniciado el 1/7/25?  
  a) El año empezó muy mal pero poco a poco la tendencia se vuelve menos negativa  
  b) El año comenzó relativamente bien pero fue empeorando con cada mes que pasaba  
  c) Los beneficios son muy estables, y no hay diferencias destacables al comparar año a año  
  d) Hay una ligera tendencia al aumento en la generación de beneficios al comparar año a año  
  e) El año comenzó muy bien, pero con el pasar de los meses esa tendencia positiva fue desmejorando


# Pasos para la solución del proyecto del día 13
1) Importa los datos, crea una tabla calculada para usar como calendario, y no olvides resolver la inconsistencia de horas que impide vincularla con las demás tablas en una relación 1 a varios.
2) Crea una matriz y coloca tu tabla de tiempo en el campo de filas.
3) Crea una medida que calcule los beneficios del año actual. Recuerda que se trata básicamente de una resta entre los precios y los costos.  
No ingreses esta medida a la matriz, ya que la consigna pide que hagamos nuestras valoraciones en función del año fiscal, por lo que aún nos falta un paso más para disponer de la medida correcta.
4) Crea otra medida para conocer los beneficios, pero esta vez del año anterior. Ten en cuenta que no es necesario volver a hacer la resta, sino que puedes tomar la medida anterior y modificar su contexto con la función CALCULATE y una función de inteligencia de tiempo.  
Tampoco agregues esta medida a la matriz. Necesitaremos hacer algunas adaptaciones previas para que podamos ver los beneficios del año fiscal (no del año calendario).
5) Ahora sí debes crear medidas que muestren el año calendario. Crea dos nuevas medidas para mostrar los beneficios (una para el año actual y otra para el anterior). Estas medidas deben utilizar una función de tiempo que permite mostrar todo lo que se ha acumulado desde el comienzo del año hasta la fecha, y en ellas debes configurar el año fiscal tal como lo pide la consigna.  
Ahora sí, agrega ambas medidas a la matriz.
6) Crea una medida que calcule la diferencia percentual respecto de los beneficios del año anterior. Recuerda que la diferencia percentual se consigue con una división.
7) Agrega un segmentador a tu informe, para poder filtrar el período que queremos que muetre nuestra matriz.
8) Ahora crea una visualización que permita ver todas las categorías de productos, y elcrecimiento (o decrecimiento) interanual de los beneficios.  
Agrega algún formato condicional para ver los registros positivos en color verde y los negativos en color rojo.

# Respuestas
1) Opción d) Electrónica para automóviles y GPS
2) Opción a) El año empezó muy mal pero poco a poco la tendencia se vuelve menos negativa