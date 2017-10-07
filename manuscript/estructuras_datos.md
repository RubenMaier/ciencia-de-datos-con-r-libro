
```r
opts_knit$set(base.dir='./', fig.path='', out.format='md')
opts_chunk$set(prompt=TRUE, comment='##', results='markup', echo=TRUE, eval=TRUE, collapse=TRUE)
# See yihui.name/knitr/options for more Knitr options.
##### Put other setup R code here


# end setup chunk
```


## Estructuras de Datos

Este capítulo resume las estructuras de datos más importantes en R. Las colecciones
o conjunto de datos en R se organizan por su dimensión (1º, 2º, o varias dimensiones)
y si son homogéneas (todos los objetos deben ser del mismo tipo) o heterogéneas (
el contenido puede ser de diferentes tipos). A continuación mostramos los cinco tipos
de datos más usados en el análisis de datos:

|  | **Homogénea** | **Heterogénea** |
| :---: | :---: | :---: |
| **1** | Vector atómico | Lista |
| **2** | Matriz | Data frame |
| **n** | Array |  |          | 

_Tabla 1 Estructuras de datos_


Además, analizaremos la sintaxis de R para acceder a las estructuras de datos. Como veremos
podemos seleccionar un único elemento o varios elementos, mediante el uso de la notación de índices que proporciona R. Asimismo
aprenderemos a elegir elementos por localización dentro de una estructura o por nombre.

La [Tabla 2]() resume los operadores que aporta R para el acceso a objetos en estructuras de datos.

| **Sintaxis** | **Objetos** | **Descripción** |
| :--- | :--- | :--- |
| __`x[i]`__ | Vectores, Listas | Selecciona elementos del objeto _x_, descritos en _i_. _i_ puede ser un vector de tipo integer, chararacter (de nombres de los objetos) o lógico. Cuando es usado con listas, devuelve una lista. Cuando es usado en vectores devuelve un vector. |
| __`x[[i]]`__ | Listas | Devuelve un único elemento de _x_ que se encuentra en la posición _i_. _i_ puede ser un vector de tipo integer o character de longitud 1. |
| __`x$n`__ | Listas, Dataframes | Devuelve un objeto con nombre _n_ del objeto _x_. |
| __`[i, j`__] | Matrices | Devuelve el objeto de la fila _i_ y columna _j_. _i_ y _j_ pueden ser un vector de tipo integer o chararacter (de nombres de los objetos) |

_Tabla 2 Notación para acceder estructuras de datos_



#### Objetivos

Después de leer este capítulo, deberíamos:

- Conocer las principales estructuras de datos que proporciona R.
- Ser capaces de crear las distintas colecciones en R.
- Saber manipular las diferentes conjuntos de datos que aporta R.
