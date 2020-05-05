# Softinn CSS Helper

A simple css helper that complements Twitter Bootstrap 3.

## Getting Started

Make sure you have referenced to Twitter Bootstrap stylesheets before you include si-css-helper.css.


### Installing

```
npm install si-css-helper
```

You may consider using WebPack to move the included si-css-helper to the folder of your web app. Below is an example we did using WebPack (TypeScript version).
```
import * as webpack from 'webpack';
import * as ExtractTextPlugin from 'extract-text-webpack-plugin';

const config: webpack.Configuration = {
    entry: [
        "./node_modules/@softinn/si-css-helper/si-css-helper.css"
    ],
    output: {
        filename: "/Content/si-css-helper.css"
    },
    module: {
        rules: [{
            test: /\.css$/,
            use: ExtractTextPlugin.extract('css-loader')
        }]
    },
    plugins: [
        new ExtractTextPlugin("./Content/si-css-helper.css")
    ]
};

export default config;
```

## Authors

The list of [contributors](https://github.com/Softinn-Solutions/si-css-helper/graphs/contributors) who participated in this project.

## License

This project is licensed under the MIT License.
