# MongoDB

Starting a MongoDB server image:

```
docker pull mongo
docker run --name mongo MONGO_INITDB_ROOT_USERNAME=root MONGO_INITDB_ROOT_PASSWORD=root -p 27017:27017 mongo
```

Creating a new database (dev):

```
docker exec -it mongo bash
mongo -u root -p root
use dev
db.test_collection.insert({"test": "test"})
```