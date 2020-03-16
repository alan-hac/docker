# Jenkins

Starting a Jenkins server image:

```
docker pull jenkins
docker run --name jenkins -p 50000:50000 -p 9000:8080 jenkins
```

Open the jenkins log and copy the token to initiate the configuration bellow
**Please use the following password to proceed to installation:** :

```
docker logs jenkins
```

Access the [local Jenkins home page](localhost:9000)

* Inform the token copied from log
* Configure a admin user and a password



