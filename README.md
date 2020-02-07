# meros-images
Docker images for the Meros cryptocurrency

## Image: Meros

[![Docker Pulls](https://img.shields.io/docker/pulls/jar013/meros)](https://hub.docker.com/r/jar013/meros)

### Running image

```shell script
mkdir data
docker run --rm -it -p 5132:5132 -p 5133:5133 -v $PWD/data/:/data/ jar013/meros:latest
```