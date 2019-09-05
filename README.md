# crx3-webpack-plugin
a webpack plugin to bundle chrome extensions for CRX3

## Inspired or enabled by the following projects:
[crx-webpack-plugin](https://github.com/johnagan/crx-webpack-plugin)
[crx3](https://github.com/ahwayakchih/crx3)

## API

add the plugin
```
yarn add crx3-webpack-plugin
```

require it:
```
const crx3 = require('crx3-webpack-plugin');
```

configure the plugin:
```
// webpack.config.js

module.exports = {
  entry: //...,
  output: //...,
  plugins: [
    new crx3({
      updateUrl: 'url-to-update.xml',
      updateFilename: 'update.xml',
      keyFile: './build.pem',
      contentPath: './build',
      outputPath: './dist',
      name: 'my-extension.crx',
   })
  ]
}
```




