# RabbitMQ

Starting a NgINX server image:

```
docker pull nginx
docker run -d --name nginx -v P:/Desenvolvimento/nginx:/usr/share/nginx/html:ro -p 80:80 nginx
```

**PS:** -v parameter shares a folder between host and vm. So you can publish static content pasting it on host folder (P:/Desenvolvimento/nginx)

Access the [local NgINX Server home page](http://localhost)