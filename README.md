# Selenium-Instagram
Código para Selenium IDE que permite la automatización de la participación en un sorteo de Instagram.


Para poder utilizar el código es necesario utilizar Google Chrome o Firefox, y tener instalado el plugin "Selenium IDE" para poder ejecutarlo.

El código se divide en varias partes...

1. Indicamos la URL del sorteo en el que queramos participar con "open", y en Target indicamos la URL.
2. Mediante "execute script" establecemos una lista en Target con los Instagrams que deseemos utilizar. Tiene el siguiente formato:
   return["@instagram1","instagram2",...].  IMPORTANTE que las cuentas almacenadas se encuentren entre "" y separadas por comas. 
   Dicha lista se almacenará dentro de de una variable, que declaramos en el campo Value. Tomemos que en este ejemplo la lista es "queso".🧀
3. Iniciamos un while con Target 1 para que este sea infinito.
4. Iniciamos un for each para que los valores de la lista queso sean sacados uno a uno en una variable llamada "varqueso". 🧀
5. Dentro del for each tenemos los pasos a realizar para poder realizar los comentarios.
6. Aplicamos 2 pausas: 1 de X tiempo para evitar una penalización de Instagram por realizar demasiados comentarios (15s), y otra más pequeña para esperar hasta que el 
   elemento del area de texto esté disponible.
7. Cerramos el for each con un end
8. Aplicamos una pausa de 10 minutos para evitar penalizaciones por parte de Instagram.
9. Cerramos el while con un end.

HAY 2 VERSIONES DISTINTAS DE ESTE CÓDIGO:

1. 4 LISTAS Y EMOJIS

2. V1, solo 1 lista... y nada mas 😛
