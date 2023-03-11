# MongoDB

## Introducción a MongoDB

### Bases de datos NoSQL

#### Documentales

En estas bases de datos se empareja cada clave con una estructura de datos compleja que se denomina 'documento'.
Otros ejemplos además de MongoDB:

- Cloud Firestore
- Couchbase

#### Grafos

Se utilizan para almacenar información sobre redes de datos, como las conexiones sociales.
Ejemplo:

- neo4j

#### Clave - Valor

Son las bases de datos NoSQL más simples. Cada elemento de la base de datos se almacena como un nombre de atributo (o "clave"), junto con su valor.
Ejemplo:

- redis

#### Orientadas a Columnas

Estas bases de datos permiten realizar consultas en grandes conjuntos de datos en columnas, en lugar de filas.
Ejemplos:

- Cassandra
- HBase

### Características de las Bases de datos NoSQL

#### Escalamiento

Las bases de datos Not Only SQL tienen gran facilidad de escalamiento.
Hay dos tipos de escalamiento.

##### Escalamiento vertical

Si tenemos una máquina y queremos soportar más capacidad o mayor velocidad, lo que hacemos es incrementar las características de esa máquina (Por ejemplo uno de sus recursos: la memoria RAM).

##### Escalamiento horizontal

Lo que hacemos es tener una máquina y copiarla o tener varios de estos nodos, lo cual asegura características como alta disponibilidad, replicabilidad o conjunto que responda en simultáneo.

##### Comparación entre escalamiento vertical y horizontal

Hacer escalamiento vertical es más fácil pero más costoso con el paso del tiempo. El escalamiento horizontal es más costoso al inicio pero luego el precio se mantiene "estándar" con el paso del tiempo.

#### Replicación

Es una técnica que, una ves distribuida la base de datos en varios nodos, mediante un load balancer asigna las peticiones y consultas a cada uno de los nodos en una forma ordenada. Esto permite procesamiento en paralelo y también alta disponibilidad (si una replica falla, habrá otra disponible). Esto no es posible en el escalamiento vertical.

#### Guía de datos no relacionales

https://azure.microsoft.com/es-es/resources/cloud-computing-dictionary/what-is-nosql-database
