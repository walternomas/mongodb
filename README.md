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

## Documentos

Son la forma en la que Mongo va a guardar la información que esté dentro de un dominio (entidad).
Ejemplos de dominios:

- Los productos de un e-commerce.
- Las clases de un curso.
- El inventario de una tienda.

Los documentos son una forma de organizar y almacenar información con un conjunto de pares **clave-valor**.

```json
{
  "name": "sue",
  "age": 28,
  "status": "A",
  "groups": ["news", "sports"]
}
```

```json
{
  "_id": "5c8eccc1caa187d17ca6ed16",
  "city": "ALPINE",
  "zip": "35014",
  "loc": {
    "y": 33.331165,
    "x": 86.208934
  },
  "pop": 3062,
  "state": "AL"
}
```

## Colecciones

Las colecciones son la forma en que guardamos los documentos y que normalmente comparten datos entre sí, o al menos sabemos que tenemos una entidad o un modelo de datos que se relacionan.

MongoDB almacena documentos en una colección, usualmente con campos comunes entre sí.

Ejemplo: Podemos tener una colección llamada Usuarios que contengan todos los documentos de los usuarios de nuestra aplicación.

## Mongo Atlas

https://www.mongodb.com/atlas

### Free Cluster

- 512 MB to 5 GB of storage.
- Shared RAM.
- Upgrade to dedicated clusters for full functionality.
- No credit card required to start.

#### Cluster

Dentro de las Tecnologías de la Información (TI), Cluster significa integrar dos o más computadoras para que trabajen simultáneamente en el procesamiento de una determinada tarea.

Saber qué es un Cluster consiste en entender que se trata de la conexión entre dos o más computadoras con el propósito de mejorar el rendimiento de los sistemas en la ejecución de diferentes tareas.

En el Cluster, cada computadora se llama “nodo”, y no hay límites sobre cuántos nodos se pueden interconectar.

Con esto, las computadoras comienzan a actuar dentro de un solo sistema, trabajando juntas en el procesamiento, análisis e interpretación de datos e información, y/o realizando tareas simultáneas.

Fuente: https://www.zendesk.com.mx/blog/cluster-que-es/

## MongoDB Compass

### Mongo Atlas

mongodb+srv://walternomas:\*\*\*\*\*@mongodb101.ircsrqb.mongodb.net/test

### Mongo Docker

mongodb://root:\*\*\*\*\*@localhost:27017/?authMechanism=DEFAULT&tls=false

## MongoDB en VSCode

https://marketplace.visualstudio.com/items?itemName=mongodb.mongodb-vscode
