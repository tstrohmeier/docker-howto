# gquintard-varnish-docker
Dockerfile for the tstrohmeier/gquintard-varnish image

I use this image for local VCL development and testing. 

@Dockerhub: https://hub.docker.com/r/tstrohmeier/gquintard-varnish/

## Pull image

``` bash
docker pull tstrohmeier/gquintard-varnish:latest

```

## What is installed in this image?
* varnish
* hitch: used to provide an endpoint with ssl
* stunnel: used in clientmode for backend endpoints with ssl or more then one IP
* socat: used for debugging the backend requests


# Build


``` bash

docker-compose build

```

# Work with the image


## Start the containers

``` bash

docker-compose up

```


## Stop the containers

``` bash

docker-compose down

```

## Reload VCL

``` bash

docker-compose exec agent varnish_reload_vcl

```

