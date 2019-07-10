# openapi

## Description
. . . .

## Available definitions
## FDSNWS - Event
Public definition:
- https://ingv.github.io/openapi/fdsnws/event/0.0.1/event.yaml

## How to *build* a definition
To build your definition from `src` file, use:
- **OpenAPI Resolver** Python module: https://github.com/ioggstream/openapi-resolver

### docker example
Build the docker following the instructions:
- https://github.com/ioggstream/openapi-resolver#use-with-docker

and run something like:
```
$ docker run -it --rm -v <absolute_path>/openapi/src/fdsnws/event/0.0.1:/code/input -v <absolute_path>/openapi/docs/fdsnws/event/0.0.1:/code/output openapi-resolver /code/input/openapi.yaml /code/output/event.yaml
```
this command will build in `<absolute_path>/openapi/docs/fdsnws/event/0.0.1` the `event.yaml` file.

## Contribute
Please, feel free to contribute.

## Author
(c) 2019 Valentino Lauciani valentino.lauciani[at]ingv.it

Istituto Nazionale di Geofisica e Vulcanologia, Italia
