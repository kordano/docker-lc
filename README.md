# Link-Collective in Docker
Dockerfile for [link-collective](https://github.com/kordano/link-collective "").

# Installation

Build it
```
[sudo] docker build --rm -t <username>/lc .
```

A couchdb instance is required for local storage.

Fill in server configuration in `opt/server-config.edn` on the local machine where docker is running.


Run it
```
[sudo] docker run -d --link couchdb:db --name lc -p 8084:8084 <username>/lc
```
