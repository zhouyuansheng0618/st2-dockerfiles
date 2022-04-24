# st2 base Docker Image
This is an intermediate Docker image with StackStorm installed in it.
We use this "base" intermediate image to build child containers for each st2 service and define granular resources like ports, volumes, users per each container.

## Build base intermediate image
```
docker build \
  --build-arg ST2_VERSION=${DOCKER_TAG} \
  --tag stackstorm/st2:${DOCKER_TAG} .
```
This is a temporary image with StackStorm packages installed in it. By default, `${DOCKER_TAG}` is set to `${ST2_VERSION}`.
