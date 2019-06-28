# openapi

## Description
. . . .

## Available definitions
## FDSNWS - Event
Public definition:
- https://ingv.github.io/openapi/fdsnws/event/0.0.1/event.yaml

## How to *build* a definition
To build your definition from `src` file, you can use:
- **docker-openapi-resolver** docker file: https://github.com/vlauciani/docker-openapi-resolver
- **OpenAPI Resolver** Python module: https://github.com/ioggstream/openapi-resolver

### docker-openapi-resolver
Build the docker following the instruction and run something like:
```
$ docker run -it --rm -v <absolute_path>/openapi/src/fdsnws/event/0.0.1:/opt/input -v <absolute_path>/openapi/docs/fdsnws/event/0.0.1:/opt/output openapi-resolver python -m openapi_resolver /opt/input/definitions.yaml /opt/output/event.yaml
```
this command will build in `<absolute_path>/openapi/docs/fdsnws/event/0.0.1` the `event.yaml` file.

### OpenAPI Resolver
Installa the Python module and run something like:
```
$ python -m openapi_resolver <absolute_path>/openapi/src/fdsnws/event/0.0.1/definitions.yaml <absolute_path>/openapi/docs/fdsnws/event/0.0.1/event.yaml
```
this command will build in `<absolute_path>/openapi/docs/fdsnws/event/0.0.1` the `event.yaml` file.

## Contribute
Please, feel free to contribute.

## Author
(c) 2019 Valentino Lauciani valentino.lauciani[at]ingv.it

Istituto Nazionale di Geofisica e Vulcanologia, Italia
