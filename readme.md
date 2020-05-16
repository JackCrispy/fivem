# FiveM

Interact with FiveM & its API with this package.

## Installation 
**Install Package**: npm i fivem

## Usage
**Examples**

Get Player Count (in numbers)
```js
const FiveM = require("fivem") // Import the npm package.
const srv = new FiveM.Server('51.38.70.222:30120') // Set the IP with port.
 
srv.getPlayers().then(data => console.log(data)) // Get & log the data!
```

Get all Resources
```js
const FiveM = require("fivem") // Import the npm package.
const srv = new FiveM.Server('51.38.70.222:30120') // Set the IP with port.
 
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

