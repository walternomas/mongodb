## Connect to container

```sh
docker-compose exec mongodb bash
```

## Connect with mongosh

```sh
mongosh "mongodb://root:root123@localhost:27017/?authMechanism=DEFAULT&tls=false"
mongosh "mongodb+srv://usuario:password@mongodb101.xcvopof.mongodb.net/test"
```

### Bases de datos disponibles

```sh
show dbs
```

### Colecciones disponibles

```sh
show collections
```

### Usar Base de datos y colección determinada

```sh
use("platzi_store")
db.products.find()
```
