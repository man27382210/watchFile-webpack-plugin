# watchFile-webpack-plugin
 * Watch file no under webpack.
 * We use ajs and rt file to build react, but webpack dev server didn't watch .rt file, so finally we wirte for watching specify folder and extension.

useage
```
watchFilePlugin = require("watchFile-webpack-plugin");
...
plugins: [
        new watchFilePlugin({watchFolder: "/src/components/", watchExtension: "rt"})
    ],
...
```

 * Which watchFolder is the folder you put the special file, and watchExtension is the extension file you look.
 * About ajs, please see [node-async-require-loader](https://github.com/jaydenlin/node-async-require-loader)!
