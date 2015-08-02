Enunciado:
El objetivo de este trabajo práctico es construir un sistema que permita realizar busquedas ranqueadas sobre una colección de documentos usando para ello el método conocido como LSI (Latent Semantic Indexing).

La colección de documentos sera un conjunto de archivos en formato texto e idioma inglés
(el idioma en realidad no es relevante).

El TP deberá procesar los documentos construyendo una matriz de terminos x documentos y luego reducir las dimensiones de la matriz a un número indicado. Ver en la web articulos sobre “Latent Semantic Indexing”, wikipedia es un buen punto de partida.

Funcionamiento del TP:

Indexar el Repositorio

Por linea de comandos un programa indexador recibe un nombre para el repositorio, un número y un directorio.

Tpgrupo17i libros -200 /home/TP/datos

El TP deberá entonces indexar todos los archivos que se encuentran en el directorio indicado, construir la matriz y reducir sus dimensiones al número indicado (en este caso 200)

Realizar Consultas

TpGrupo17q -r libros -q sherlock holmes apple

El TP recibe como parametros el nombre del repositorio a consultar y una lista de términos (palabras) y debe devolver una lista con todos los documentos de la colección ordenados por relevancia. El documento mas relevante para la consulta primero.


Evaluación:

Los Tps serán evaluados en base a la calidad del ranqueo para diferentes dimensiones. El grupo cuyo TP funcione mejor recibe 10 puntos que pueden ser usados en el examen por promoción o bien en el segundo recuperatorio.


Importante:


–El TP debe desarrollarse en C o C++ exclusivamente.

-El TP debe desarrollarse bajo Linux y será probado bajo Linux.

-Para el proceso de reducción de dimensiones de la matriz se puede usar código libre o
programas auxiliares en otros lenguajes.