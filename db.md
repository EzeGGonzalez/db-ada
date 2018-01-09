# Base de datos

## ¿Qué es una base de datos?
* Una base de datos es una colección de datos organizados según un determinado criterio
* Estos datos se pueden leer, crear, actualizar y borrar
* También existen motores de base de datos que nos permiten hacer todas estas operaciones de forma más fácil

### Tipos de base de datos
* Existen distintos tipos de bases de datos que se utilizan para solucionar distintos tipos de problemas
* Dentro de la gran familias de bases de datos podemos encontrar las del tipo base de datos relacionales y las no relacionales
* Las bases de datos relacionales se conocen generalmente como las SQL
* Las no relacionales se conocen como NoSQL
* Cada tipo de base de datos tiene beneficios y contras a la hora de almacenar, leer, actualizar o borar los datos

### Bases de datos relacional
> La base de datos relacional (BDR) es un tipo de base de datos (BD) que cumple con el modelo relacional

* Desde su definición vemos que una base de datos puede ser [relacional](https://es.wikipedia.org/wiki/Base_de_datos_relacional) si cumple con algo conocido como el [modelo relacional](https://es.wikipedia.org/wiki/Modelo_relacional)

> El modelo relacional es un modelo de datos basado en la lógica de predicados y en la teoría de conjuntos. Su idea fundamental es el uso de relaciones. Estas relaciones podrían considerarse en forma lógica como conjuntos de datos llamados tuplas. Pensamos cada relación como si fuese una tabla que está compuesta por registros (cada fila de la tabla sería un registro o "tupla") y columnas (también llamadas "campos").

* En la definición de modelo relacional nos podemos quedar con la idea de tablas que tienen columnas para describir los datos que están relacionados entre si.
#### Ejemplo modelo relacional:
![Modelo Relacional](../assets/db/modelo-relacional.jpg)

* Para que sea modelo relacional debe cumplir con los [siguientes requisitos](https://es.wikipedia.org/wiki/12_reglas_de_Codd)
* Entre los motores de bases de datos relacionales más conocidas encontramos a [SQL Server](https://www.microsoft.com/es-es/sql-server/sql-server-2016), [MySQL](https://www.mysql.com/) y [PostgreSQL](https://www.postgresql.org/) entre otras
* Estos motores de base de datos soporta el [lenguaje SQL](https://es.wikipedia.org/wiki/SQL) (Structured Query Language) para realizar consultas
* Este modelo de datos es el más utilizado en la actualidad
* Para completar nuestra formación como profesionales está muy bueno incorporar conocimientos sobre este tipo de bases de datos
* Uno de los grandes beneficios que tiene este tipo de motores de base de datos es poder realizar [operaciones atómicas](https://es.wikipedia.org/wiki/Atomicidad)
* Evita tener datos repetidos
* Escala de manera vertical
* Para aprender más sobre SQL pueden ingresar a los sitios de:
  * [Fundamentos SQL](http://pedrobeltrancanessa-biblioteca.weebly.com/uploads/1/2/4/0/12405072/fundamentos_de_sql_3edi_oppel.pdf)
  * [Khan Academy (inglés)](https://www.khanacademy.org/computing/computer-programming/sql)
  * [W3 Schools (inglés)](https://www.w3schools.com/sql/)

### Modelo NoSQL
* Se conoce como [NoSQL (Not Only SQL)](https://es.wikipedia.org/wiki/NoSQL) al grupo de bases de datos que no son relacionales
* Dentro de esta clasificación se encuentran las bases de clave/valor, orientadas a documentos, grafos, de grandes columnas
![NoSQL](../assets/db/nosql.png)
* Este tipo de bases de datos escala de forma horizontal
* Podemos utilizar muchas máquinas chiquitas para crecer y satisfacer las necesidades de los negocios actuales

![Escalar](../assets/db/escalar.png)

#### Clave/valor
* Las bases de datos de `clave/valor` guardan valores en formato de diccionario o hash utilizando una clave como índice y su valor. 

![Clave/Valor](../assets/db/key-value.png)

#### Orientadas a documentos
* Las base de datos `orientadas a documentos` es bastante parecída a las de `clave/valor`.
* La diferencia recide principalmente en en la complejidad del modelo de dato
* Clave/valor tiene un modelo de lo más simple
![SQL v NoSQL](../assets/db/SQLvsNoSQL.png)

* Documento puede tener un modelo de documento complejo
* Muchos de estos motores utilizan JSON/BSON para guardar los datos
![NoSQL](../assets/db/document.svg)
* Entre los motores más conocidos de este tipo se encuentra MongoDB

#### Grafos
* Estas bases de datos utilizan el modelo de Grafos
* Se especializan en relaciones
* Las podemos utilizar por ejemplo para guardar puntos de un camino, relaciones de amigos, familia, o cualquier tipo de dato que represente alguna relación
* Entre los motores más conocidos de este tipo se encuentra Neo4j

![Grafo](../assets/db/graph.png)

#### Grandes columnas/BigTable
* Este tipo de familia de bases de datos está orientada a grandes cantidades de datos
* Lo datos son almacenados en columnas
* En una columna tiene múltiples datos
* Entre los motores más conocidos de este tipo se encuentra Cassandra o HBase
![Base de datos de columnas](../assets/db/column-oriented-database.jpg)

* Podemos informarnos más sobre las diferencias entre SQL y NoSQL en el [siguiente link](https://blog.pandorafms.org/es/nosql-vs-sql-diferencias-y-cuando-elegir-cada-una/)

## MongoDB
* MongoDB es una base NoSQL orientada a documentos
* Permite guardar documentos en formato de JSON
* Tiene esquema flexible, es decir que podemos cambiar la estructura de nuestros documentos sin ningún problema
* MongoDB está preparado para escalar fácilmente de manera horizontal
* Dado que aprendimos ECMAScript vamos a utilizar un motor de base de datos que nos permite seguir utilizando este lenguaje para guardar nuestros datos