# RabbitMQ

Starting a RabbitMQ server image:

```
docker pull rabbitmq
docker run -d --hostname rabbit --name rabbitmq -e RABBITMQ_DEFAULT_USER=admin -e RABBITMQ_DEFAULT_PASS=admin -p 15672:15672 rabbitmq:management
```

Access the [local RabbitMQ Management home page](localhost:15672)