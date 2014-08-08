# Swagger CLI Client

Generates a command-line interface for any 
[Swagger Specification](https://github.com/wordnik/swagger-spec/blob/master/versions/1.2.md) so you can do things like:


## Usage
This intended to be embedded within a wrapper application which can provide it the schema object (which is generated using [fetch-swagger-schema](https://github.com/signalfuse/fetch-swagger-schema)). For example, here's the petstore-cli file:

```javascript
#!/usr/bin/env node

var swaggerCli = require('../'),
  schema = require('./petstore-schema.json');

swaggerCli(schema);
```

To create a cli app for your schema, just require your schema instead of the petstore schema.
