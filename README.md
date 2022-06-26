# Selenium-Instagram
Código para Selenium IDE que permite la automatización de la participación en un sorteo de Instagram.


Para poder utilizar el código es necesario utilizar Google Chrome o Firefox, y tener instalado el plugin "Selenium IDE" para poder ejecutarlo.

El código se divide en varias partes...

1. Indicamos la URL del sorteo en el que queramos participar con "open", y en Target indicamos la URL.
2. Mediante "execute script" establecemos una lista en Target con los Instagrams que deseemos utilizar. Tiene el siguiente formato:
   return["@instagram1","instagram2",...].  IMPORTANTE que las cuentas almacenadas se encuentren entre "" y separadas por comas. 
   Dicha lista se almacenará dentro de de una variable, que declaramos en el campo Value. Tomemos que en este ejemplo la lista es "queso".
3. Iniciamos un while con Target 1 para que este sea infinito.
4. Iniciamos un for each para que los valores de la lista queso sean sacados uno a uno en una variable llamada "varqueso".
5. Dentro del for each tenemos los pasos a realizar para poder realizar los comentarios.
6. Aplicamos 2 pausas: 1 de X tiempo para evitar una penalización de Instagram por realizar demasiados comentarios (15s), y otra más pequeña para esperar hasta que el 
   elemento del area de texto esté disponible.
7. Cerramos el for each con un end
8. Aplicamos una pausa de 10 minutos para evitar penalizaciones por parte de Instagram.
9. Cerramos el while con un end.


CONSEJOS:
1. Es recomendable que las listas NO superen los 15 usuarios, ya que con los tiempos predefinidos, Instagram puede realizar una penalización.
2. Podemos aplicar tantas listas como queramos, solo tenemos que inicializar cada lista como se ve con la primera, y hacer copy paste del for each (DENTRO DEL WHILE) de manera consecutiva para poder utilizar dichas listas, aplicando siempre 10 minutos de pausa entre cada uno de los for each.

OBSERVACIONES:
1. Este es un código que hice super rapido para participar en un sorteo (yo no he ganado nada por ahora, pero mis hermanos usando el código si...), por lo que puede que sea un poco desastre. Si al utilizar el código, realizas unas optimizaciones óptimas, estaría bien que las compartas, ya que me ayudaría a mí y al resto.
2. Estoy buscando la manera de poder llevar a cabo la misma idea para Twitter y Facebook (aunque Twitter es más complicado), por lo que puede que también lo suba por aquí.
3. No se que más decir haha, solo que sub a LICK 123 :)
