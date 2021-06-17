# Softinn CSS Helper

A simple css helper that complements Twitter Bootstrap 3. Added flex box support too.

## Getting Started

1. Add reference to Bootstrap 3 https://getbootstrap.com/docs/3.3/
2. Make a copy of si-css-helper.min.css to your project

### NPM Install

```
npm install @softinn-solutions/si-css-helper
```

### Other Suggestions
If you're using the npm package, you may consider using WebPack to copy the si-css-helper.css to the folder of your web app. Below is an example code example (implemented using TypeScript).
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
