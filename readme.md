# FiveM

API for getting FiveM server info & status.

## Installation 
**Install Package**: npm i fivem

## Usage
**Examples**

See if server is online (json)
```js
const FiveM = require("fivem") // Import the npm package.
const srv = new FiveM.Server('IP:PORT') // Set the IP with port.
 
srv.getServerStatus().then(data => console.log(data)) // Get & log the data!

//if online returns json {online: true}
// if offline returns json {online: false, url: x, method: x}
```

Get Player Count (in numbers)
```js
const FiveM = require("fivem") // Import the npm package.
const srv = new FiveM.Server('IP:PORT') // Set the IP with port.
 
srv.getPlayers().then(data => console.log(data)) // Get & log the data!
```

Get all Resources
```js
const FiveM = require("fivem") // Import the npm package.
const srv = new FiveM.Server('IP:PORT') // Set the IP with port.
 
srv.getResources().then(data => console.log(data)) // Get & log the data!
```

## **ALL FUNCTION REQUESTS**
- getPlayers - (number)
- getMaxPlayers - (number)
- getResources - (string/array)
- getTags - (string)
- getServer - (string)
- getOnesync - (boolean)
- getLocale - (string)
- getGamename - (string)
- getEnhancedHostSupport - (boolean)
- getlicenseKeyToken - (string)
- getScriptHookAllowed - (boolean)

