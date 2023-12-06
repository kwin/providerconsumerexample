This is a reactor containing an API bundle exporting a consumer and provider type (the former inheriting from the latter).

In addition two dependent modules.
One only extending the consumer and the other one also implementing the provider.
Although the effectively implemented interfaces are the same (through inheritance) the import-version range differs.

It looks like this for dependent-module1:

```
Import-Package: org.example.api;version="[1.0,2)"
```

while it looks like this for dependent-module2:

```
Import-Package: org.example.api;version="[1.0,1.1)"
```