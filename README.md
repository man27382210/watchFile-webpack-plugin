[![Build Status](https://travis-ci.org/man27382210/watchFile-webpack-plugin.svg?branch=master)](https://travis-ci.org/man27382210/watchFile-webpack-plugin)
# watchFile-webpack-plugin
 * Watch file not under webpack.
 * We use ajs and rt file to build react, but webpack dev server didn't watch `*.rt` files, so finally we wrote this plugin for watching files within a specific folder and extension.

useage
```
watchFilePlugin = require("watchfile-webpack-plugin");
...
plugins: [
  new watchFilePlugin({watchFolder: "/src/components/", watchExtension: "rt"})
],
...
```

 * Which watchFolder is the folder you put the special file, and watchExtension is the extension file you look.
 * About ajs, please see 
   * [node-async-require-loader](https://github.com/jaydenlin/node-async-require-loader)
   * [node-async-require](https://github.com/jaydenlin/node-async-require)
