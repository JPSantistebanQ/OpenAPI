# OpenAPI

In this repo we will learn with examples how to use OpenAPI to document your APIs.

## Schema object

The Schema Object allows the definition of input and output data types. These types can be objects, but also primitives and arrays.

```yaml
openapi: 3.0.0
info:
  title: Sample API
  version: 1.0.0
paths:
```

## Components Object

The Components Object allows you to define reusable objects for your API.

```yaml
components:
  schemas:
    User:
      type: object
      properties:
        id:
          type: integer
          format: int64
        name:
          type: string
        email:
          type: string
          format: email
```

### Fields

| Field Name | Type | Description |
|------------|------|-------------|
| schemas | Map[string, Schema Object] | An object to hold reusable Schema Objects. |
| responses | Map[string, Response Object] | An object to hold reusable Response Objects. |
| parameters | Map[string, Parameter Object] | An object to hold reusable Parameter Objects. |
| examples | Map[string, Example Object] | An object to hold reusable Example Objects. |
| requestBodies | Map[string, Request Body Object] | An object to hold reusable Request Body Objects. |
| headers | Map[string, Header Object] | An object to hold reusable Header Objects. |
| securitySchemes | Map[string, Security Scheme Object] | An object to hold reusable Security Scheme Objects. |
| links | Map[string, Link Object] | An object to hold reusable Link Objects. |
| callbacks | Map[string, Callback Object] | An object to hold reusable Callback Objects. |

