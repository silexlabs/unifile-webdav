# Unifile WebDAV

This is a plugin for [Unifile](https://github.com/silexlabs/unifile) to use WebDAV services with it.

To include it in Unifile, you first need to install it
```bash
# Node 6+
$ npm install unifile-webdav -S

# Node 8+
$ npm install unifile-webdav
```

Then, you'll have to register it to unifile
```javascript
const Unifile = require('unifile');
const UnifileWebDAV = require('unifile-webdav');

const unifile = new Unifile();

// Register a new connector
unifile.use(new UnifileWebDAV({redirectUri: 'http://localhost:3000/callback'}));
```
