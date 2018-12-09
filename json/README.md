## Preparation
docker build -t docker-flask-examples-json .

## Start the server
docker run --rm -p 5000:5000 docker-flask-examples-json

## Use API
```sh
$ curl localhost:5000/
{"foo":"bar","ほげ":"ふが"}
$ curl -X POST -H 'Accept:application/json' -H 'Content-Type:application/json' -d '{"data":"hoge"}' localhost:5000/
{"data":"hoge"}
```
