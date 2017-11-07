# To Be Studied

* Saga, sagas test
* Setup, mokea, babellish
* Jenkins
* Webpack buildingDll
* ngrok
* swagger

# To Be Explained

* Injectors, ex : injectReducer() see app/pages/Events, why loading reducers dynamically ?
* why SSR ? to change favicon, deeplinking on page !!
* Best practices 
* setPropTypes



# To Be Defined

* how to test hoc wrapped components ? shallow() + dive() ou mount(), ...

# To Be refactored

* ramda, lodash, Immutable => ramda, care settings seams to use immutable even in components
* SSR
* bundle process + server => use CRA + peep
* use evtX
* ~~use Prettier~~
* config client and server

# SSR
* remove generated files (generated.assets.json  generated.serverEntry.js)
* use app-module-path to add app in module path
```
const modulePath = path.join(__dirname, '../app/')
require('app-module-path').addPath(modulePath);
```
* use `ignore-styles`for css, cvg, ... (assets)
* setup babel with latest, ...

```
$ babel-node server/devRenderService.js 
```

TODO:

* integrate devRenderService in main server
* use webpack config from CRA
* find a solution to get svg at first page load (bundle with webpack, migrate to css)

