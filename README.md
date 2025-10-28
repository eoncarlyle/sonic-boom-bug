# Sonic Boom Bug

The only difference between 'standard' and 'special' is that special replaces the
'u' in the first line with 'ü'.

```shell
$ npm run standard

> sonic-boom@1.0.0 standard
> node index.js

First 10 chars: {"level":"
Last 10 chars: 266:abcdef
First 10 chars: ghijklmnop
Last 10 chars: Received"}
```

```shell
$ npm run special

> sonic-boom@1.0.0 special
> node index.js special

First 10 chars: {"level":"
Last 10 chars:
266:abcde
First 10 chars: ghijklmnop
Last 10 chars: Received"}
```
