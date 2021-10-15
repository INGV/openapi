# openapi

## Description
This project contains OpenAPI-3 definitions and common definitions used at INGV.

## Available definitions in OpenAPI-3
### FDSNWS - Event
Event (earthquake) information in QuakeML and text format
- (definition) https://ingv.github.io/openapi/fdsnws/event/0.0.1/event.yaml
- (API) http://webservices.ingv.it/fdsnws/event/1/

### Shakedata
ShakeMap input Intensity Measure data extracted from recorded waveforms
- (definition) https://ingv.github.io/openapi/fdsnws/shakedata/0.0.1/shakedata.yaml
- (API) http://webservices.ingv.it/ingvws/shakedata/1/

## INGV common definitions
When you document an API, it is common to have some features which you use across several of API resources. In that case, you can create a snippet for such elements in order to use them multiple times when you need it. With OpenAPI 3.0, you can reference a definition hosted on any location. It can be the same server. 

To reference a definition, use the `$ref`.

#### Common INGV definitions
- https://ingv.github.io/openapi/definitions.yaml

#### Earthworm software
- https://ingv.github.io/openapi/definitions_ew.yaml

### How to use:
Example:
```
    Origin:
      type: object
      properties:
        id:
          $ref: 'https://ingv.github.io/openapi/definitions.yaml#/components/schemas/id'
        ot:
          $ref: 'https://ingv.github.io/openapi/definitions.yaml#/components/schemas/origin__ot'
        lat:
          $ref: 'https://ingv.github.io/openapi/definitions.yaml#/components/schemas/latitude'
```

## Contribute
Please, feel free to contribute.

## Author
(c) 2021 Valentino Lauciani valentino.lauciani[at]ingv.it

Istituto Nazionale di Geofisica e Vulcanologia, Italia
