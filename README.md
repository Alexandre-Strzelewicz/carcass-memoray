# Carcass Memoray

Storage plugin for Carcass using [ArrayJS](http://matthewmueller.github.com/array/)

## Methods

- put(data, cb)
- find(data, cb)
- del(data, cb)

## Example

/!\ Don't forget to require('carcass-memoray') in the index.js carcass root file.

```
var storage = carcass.storages.memoray({
    id: 'model'
});

var builder = carcass.factories.Model({
    attributes: {
        id: {},
        username : {}
    },
    storage: storage
});

builder.use(carcass.plugins.modelSync);

```
## Test

`make test`
