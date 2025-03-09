# Consigna para el Proyecto del Día 9
Suficientes aprendizajes por hoy ¿verdad? Me he quedado con ganas de mostrarte un par de temas más en Power Query, pero los vamos a dejar para mañana, que es un día que también se trae cosas nuevas y muy interesantes. Valoro mucho todo el esfuerzo que has realizado para llegar hasta aquí, y creo que ya es un buen momento para que pongas en práctica lo aprendido.  
El día de hoy te voy a presentar 3 archivos con información que vas a usar para representar la evolución de las cotizaciones de las acciones de 5 empresas muy importantes, todas ellas de algún modo ligadas a la tecnología y la innovación.  
Tu objetivo consistirá en tomar los dos archivos XML que contienen los datos diarios del precio de la acción en un periodo determinado, y deberás combinarlos en una única tabla de datos, de modo tal que finalmente puedas graficar el periodo completo en una sola visualización de Power BI.  
Sin embargo, para que la información sea más interpretable para un público general, te pediré que, a través de combinaciones y transformaciones en Power Query, logres representar el nombre de cada empresa y sus símbolos de cotización de la siguiente manera. Este es el ejemplo para el caso de TESLA:  
<code> Tesla Inc (TSLA) </code>  
Es decir, el nombre de la empresa, y entre paréntesis el nombre de su símbolo en la bolsa.  
Una advertencia con relación a este proyecto: vas a necesitar usar tu creatividad para explorar herramientas y resolver problemas, así como para recordar todas las estrategias de transformación y procesamiento de datos en las que hemos trabajado tanto ayer como hoy. Recuerda que puedes verificar los datos de origen en el bloc de notas para revisar que la importación se realice correctamente y con la configuración regional adecuada. Recuerda también que tus datos deben tener una forma determinada para poder graficarse correctamente.  

# Pasos para la solución del proyecto del día 9
1) Carga los 3 archivos que te he dejado en los recursos de la lección. Luego abre el editor de Power Query y observa los datos que tienes a tu disposición, su estructura y las posibilidades de relacionarlos entre sí.
2) Anexa las tablas que provienen de los archivos XML, para que todos los registros de valores de bolsa queden listados en una sola tabla. Una vez hecho esto puedes deshabilitar la carga de la tabla que ha quedado obsoleta.
Con esto podrás responder a las preguntas 1 y 2
3) En la tabla resultante de la anexión, si es necesario para ti, corrige los problemas de configuración regional que se hayan presentado (insisto: esto solamente si los datos no coinciden con la configuración de tu ordenador).
4) En la tabla que contiene los nombres y símbolos de las empresas, primero asegúrate de que los encabezados de columnas sean los correctos, y luego crea una nueva columna que sea el resultado de combinar los valores de las dos columnas anteriores. Debes hacer esto de forma tal que la estructura del valor resultante sea la siguiente:  
nombre (símbolo)  
Ten presente que para lograrlo, debes explorar las posibilidades que ofrecen las herramientas de formato tanto de la etiqueta Transformar, como de la etiqueta Agregar columna.
5) Ahora ya puedes combinar ambas tablas, y asegurarte de expandir solamente la que contiene el valor de etiqueta que has creado.  
Una vez que hagas esto, tambien puedes deshabilitar la carga de la tabla de los nombres.
6) Carga tus datos al modelo, y procura crear una visualización que despliegue la información de un modo comprensible.