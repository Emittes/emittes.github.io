# No Key Provided Error

## Cause
The Key Provided error is thrown when you fail to provided a token or key provided by emittes control server.

## Fix

Ensure when your are calling the EmittesIO class correctly with the token, Like Below:
```node
const EmittesIO = require('EmittesIO')
const io = new EmittesIO({'key': 'ADD KEY HERE'});
```
