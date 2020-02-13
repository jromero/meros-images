# meros-images
Docker images for the Meros cryptocurrency

## Image: Meros

[![Docker Pulls](https://img.shields.io/docker/pulls/meroscrypto/meros)](https://hub.docker.com/r/meroscrypto/meros)

### Running image

```shell script
mkdir data
docker run --rm -it -p 5132:5132 -p 5133:5133 -v $PWD/data/:/data/ meroscrypto/meros:latest
```

## Image: Mineros

[![Docker Pulls](https://img.shields.io/docker/pulls/meroscrypto/mineros)](https://hub.docker.com/r/meroscrypto/mineros)

### Running image

```shell script
docker run --rm -it --net="host" meroscrypto/mineros:latest localhost 5133
```