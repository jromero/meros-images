# meros-images
Docker images for the Meros cryptocurrency

## Running Meros image

```shell script
mkdir data
docker run --rm -it -p 5132:5132 -p 5133:5133 -v $PWD/data/:/data/ meros:latest
```