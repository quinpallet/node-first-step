# node-first-step

For testing/studying JavaScript using Node.js runtime environment

## Usage

JS file running on Node.js should be in 'src' directory.

```sh
$ docker-compose run [-d] --rm app node test.js
```


## restify

[restify](https://github.com/restify/node-restify) framework for building Node.js REST APIs.

### Prerequisites
```sh
$ docker-compose run --rm app npm i restify restify-clients
```

### Server
```sh
$ docker-compose run -d --rm app node restify-server.js
```

### Client
```sh
$ docker-compose run --rm app node restify-client.js
```
OR
```sh
$ curl -is http://localhost:8080/echo/mark
```


## fastify

[fastify](https://github.com/fastify/fastify) framework for building Node.js REST APIs.

### Prerequisites
```sh
$ docker-compose run --rm app npm i fastify
```

### Server
```sh
$ docker-compose run -d --rm app node fastify-server.js
```

### Client
```sh
$ curl -is http://localhost:3000
```
