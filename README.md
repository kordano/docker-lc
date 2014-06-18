# Link-Collective in Docker
Dockerfile for [link-collective](https://github.com/kordano/link-collective "").

# Installation

Build it
```
[sudo] docker build --rm -t <username>/link-collective .
```

A couchdb instance is required for local storage.

Fill in server configuration in `opt/server-config.edn` on the local machine where docker is running.


Run it
```
[sudo] docker run -t -i --link couchdb:db --name link-collective -p 8080:8080 <username>/link-collective
```
