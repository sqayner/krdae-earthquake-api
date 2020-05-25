# KRDAE EARTHQUAKE API (NODE.JS)


## USAGE
1. Add [request-promise](https://www.npmjs.com/package/request-promise) library to your project. You can use `> npm i request-promise`
2. Earthquake.js file add to project root
3. Add the following code to the index.js file.
```javascript
const apiEarthquake = require('./earthquake')

apiEarthquake()
    .then(count => {
        console.log(JSON.stringify(count))
    })
    .catch(err => {
        console.log(err)
    })
```
4. You can use it to start your project `> npm start` or `> node index.js`

## EXAMPLE RESPONSE
```
{
    result: [
	{
            magnitude: "2.5",
            latitude: "38.3335",
            longitude: "44.3443",
            location: "GELENLER-BASKALE(VAN)",
            depth: "6.9",
            timestamp: 1590426749,
            time: "2020.05.25 17:12:29"
        },
        {
            magnitude: "3.2",
            latitude: "34.2502",
            longitude: "25.5082",
            location: "GIRITADASIACIKLARI(AKDENIZ)",
            depth: "7.8",
            timestamp: 1590419087,
            time: "2020.05.25 15:04:47"
        },
        ...
    ]
}
```
