# MongoDB

Starting a MongoDB server image:

```
docker pull mongo
docker run --name mongo -e MONGO_INITDB_ROOT_USERNAME=root -e MONGO_INITDB_ROOT_PASSWORD=root -p 27017:27017 mongo
```

Creating a new database (app):

```
docker exec -it mongo bash
mongo -u root -p root
use app
db.test_collection.insert({"test": "test"})
```

Creating a exclusive user for app db:

```
db.createUser(
  {
    user: "appUser", 
    pwd: "app123456", 
    customData: { 
      "description": "Application database" 
    }, 
    roles: [ 
      { 
        role: "readWrite", 
        db: "app" 
      }
     ]
  }
) 
