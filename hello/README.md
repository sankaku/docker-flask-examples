## Preparation
docker build -t docker-flask-examples-hello .

## Start the server
docker run --rm -p 5000:5000 docker-flask-examples-hello

## Use API
```sh
$ curl localhost:5000/hello
{"message":"Hello, world"}

$ curl --head localhost:5000/hello
HTTP/1.0 200 OK
Content-Type: application/json
Content-Length: 27
Server: Werkzeug/0.14.1 Python/3.7.1
Date: Sun, 09 Dec 2018 03:03:20 GMT
```
