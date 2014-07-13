# Topiq in Docker
Dockerfile for [topiq](https://github.com/kordano/topiq"").

# Installation

Build it
```
sudo docker build --rm -t <username>/topiq .
```

A couchdb instance is required for local storage.

Fill in server configuration in `opt/server-config.edn` on the local machine where docker is running.


Run it
```
sudo docker run -d --link couchdb:db --name topiq -p 8084:8084 <username>/topiq
```
