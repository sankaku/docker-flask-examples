## Preparation
docker build -t docker-flask-examples-routing .

## Start the server
docker run --rm -p 5000:5000 docker-flask-examples-routing

## Use API
```sh
$ curl localhost:5000/foo/bar
you got

$ curl -X POST localhost:5000/foo/bar/42
you posted 42
```
