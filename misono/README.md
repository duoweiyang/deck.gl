This is a data visualization project based on the code from the [deck.gl](http://deck.gl) website.
The goal is to create an animated image showing the data collected from smart houses in Urawa-Misono over the course of a year. 

### Usage
- Copy the content of this folder to your project.

- Install Package
```
npm install
```

- Delete last line in `webpack.config.js`
```
module.exports = require('../webpack.config.local')(module.exports);
```

- Add [Mapbox access token](https://www.mapbox.com/help/define-access-token/)
by run this command in your terminal.

```
export MapboxAccessToken=<Your_Token>
```

or you can directly add it to `app.js`
```
// Set your mapbox token here
const MAPBOX_TOKEN = <Your_Token>>;
```
- Start the app.
```
npm start
```

### Data format
Sample data is stored in [deck.gl Example Data](https://github.com/uber-common/deck.gl-data/tree/master/examples/3d-heatmap). To use your own data, checkout
the [documentation of HexagonLayer](../../docs/layers/hexagon-layer.md)
