# Postgresql:9.6 container for 512 CUBE dimensions

The cube extension, which you'll use to perform operations on vectors, has a hard limit of 100 dimensions per vector.
This container has an increased limit of 512 dimensions.

## Architecture
* AMD64
* ARM

## Build & start

### AMD64 (default)
docker build --no-cache -t diduxio/pg512d:latest .
docker run --rm  --name postgres -e POSTGRES_PASSWORD=docker -d -p 5432:5432 diduxio/pg512d:latest

### ARM
docker build --no-cache -t diduxio/pg512d:arm -f Dockerfile-arm .
docker run --rm  --name postgres -e POSTGRES_PASSWORD=docker -d -p 5432:5432 diduxio/pg512d:arm

### Connecting
```psql -h localhost -U postgres -d postgres```

## Push (for owners of this repository)
docker push diduxio/pg512d:latest
docker push diduxio/pg512d:arm

