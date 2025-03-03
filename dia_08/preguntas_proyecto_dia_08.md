# Consigna para el Proyecto del Día 8
Llegó la hora de dedicarnos por completo a poner en práctica los conocimientos adquiridos en este día. Como seguro te lo estás imaginando, hoy  vamos a trabajar exclusivamente en Power Query. Y el desafío que tienes por delante es el de procesar y transformar una base de datos que te vas a descargar de esta lección, pero que tiene varios errores, y no te voy a decir cuáles son.  
Entonces, limpia los datos, y a luego de eso aplica transformaciones de modo tal que puedas responder a las preguntas que también te voy a dejar para que te descargues.  
La consigna, es que crees un código de usuario a partir de las iniciales del nombre completo de la persona, y luego un número que se corresponda con su orden de registro. El número debe partir de 1001, y seguir la cuenta agregando una unidad (es decir que le sigue 1002, 1003, y así… en función del orden en que los usuarios fueron ingresando).  
Entonces por ejemplo, si el primer usuario que ingresó se llama Alberto Blas Correa, su código debería ser ABC1001.  

# Preguntas
1) ¿Qué código tiene asignado Tomás Burgos Gutiérrez?
2) ¿Qué código tiene asignado César Reyes Villanueva?
3) Al día 31/12/2023, ¿qué antigüedad (expresada en años) tiene Laura Cordero Martínez? Ayúdate con la columna auxiliar.

# Pasos para la solución del proyecto del día 8
1) Luego de cargar el archivo y abrir el editor de Power Query, realiza la limpieza de datos eliminando las columnas y filas innecesarias, y produciendo los encabezados correctos. Revisa los tipos de datos de cada campo y explora tus datos para verificar con qué recursos cuentas.
2) Para crear la columna de códigos necesitarás ordenar tus registros por fecha de ingreso. El resto del trabajo podría dividirse en dos partes:  
a- Crear una columna que contenga las iniciales en mayúscula de los usuarios. Esto implica modificar el formato (mayúsculas) y encontrar la manera de extraer las iniciales de cada palabra del nombre.  
b- Crear otra columna que asigne a cada registro un número. El primero debe ser 1001 y los siguientes deben aumentar de 1en 1.  
No olvides combinar ambas columnas cuando lo hayas hecho.  
Con esto podrás responder a las preguntas 1 y 2
3) Para responder a la tercera pregunta debes modificar la fecha de la columna auxiliar para que represente a la fecha indicada. Luego debes calcular los días transcurridos desde el ingreso de cada usuario hasta la fecha solicitada, y transformar el resultado en un dato de tipo duración.  
Finalmente debes hacer que esa duración se exprese en años.  
Un vez terminado, encontrarás la respuesta a la pregunta 3.

# Respuestas
1) TBG1030
2) CRV1016
3) 1183