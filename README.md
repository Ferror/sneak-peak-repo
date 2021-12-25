# sneak-peak-repo
## Introdcution

There are SOAP and gRPC patterns that has really nice feature. **Contract**. It makes a lot of things easier,
but SOAP requires old WSDL defined in XML and gRPC nice Protocol Buffers that requires special definition.

Why can we just use JSON instead?!

Contract definition example.

```json
{
    "entity": {
        "key-string": "@string",
        "key-integer": "@integer",
        "key-boolean": "@boolean",
        "key-array": "@array", //todo array of integers, strings, booleans...
        "key-object": "@object-name",
        "enum": "VALUE1|VALUE2"
    }
}
```

Giving the JSON contract we should be able to generate client and server files just like in the gRPC Protocol Buffers
