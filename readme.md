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
- getPlayers - Number of players online - (number)
- getPlayersAll - List all players in an array - (string)
- getMaxPlayers - Max players that are able to join the server - (number)
- getResources - Get resource names of all server resources - (string/array)
- getTags - Get all server tags - (string)
- getServer - Get the whole server object - (string)
- getOnesync - See if the server has OneSync enabled - (boolean)
- getLocale - The language of the server - (string)
- getGamename - Get the name of the server - (string)
- getEnhancedHostSupport - ... - (boolean)
- getlicenseKeyToken - The license key for the server - (string)
- getScriptHookAllowed - See if the server supports external mod menus from the client - (boolean)

