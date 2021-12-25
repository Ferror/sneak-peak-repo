# sneak-peak-repo
## Introdcution

There are SOAP and gRPC patterns that has really nice feature. Contract. It makes a lot of things easier,
but SOAP requires old WSDL defined in XML and gRPC requires protbufs and special definition.

Can we like use JSON instead, cause we love it!

Contract definition example

```json
{
    "entity": {
        "key-string": "@string",
        "key-integer": "@integer",
        "key-boolean": "@boolean",
        "key-array": "@array", //todo array of integers, strings, booleans...
        "key-object": "@object-name"
    }
}
```
