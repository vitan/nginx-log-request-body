# nginx-log-request-body

## how to use it

1. start the container and echo the log forcely

```bash
docker logs -f `docker run -p 80:80 -d nginx-log-request-body:latest`
```

2. post the test data to the nginx server
```bash
curl -X POST http://localhost:80/post -d 'test'
```
