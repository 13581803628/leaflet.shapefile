leaflet.shapefile
=================

如果你想在你的程序中运行这个插件，你必需加载 [shapefile-js](https://github.com/calvinmetcalf/shapefile-js) 文件。你可能会用到 [catiline](https://github.com/calvinmetcalf/catiline)。

**用法：**

```javascript
new L.Shapefile(arrayBuffer or url[,options][,importUrl]);

L.shapefile(arrayBuffer or url[,options][,importUrl]);
```

参数会按照原样传递给 `L.Geojson` 方法。 第一个参数是shapefile压缩文件的阵列缓存（array buffer），或者是shapefile压缩文件的URL地址，或者是shape文件（.shp）的URL地址（要求dbf文件同时存在）。`importUrl` 参数允许你在使用[catiline](https://github.com/calvinmetcalf/catiline)时改变`shp.js`在哪里加载程序，默认情况下为 `shp.js`。

为了使你用自己的shapefile文件测试这个库更简单，查看 [leaflet.calvinmetcalf.com](http://leaflet.calvinmetcalf.com/)上的在线示例, 在这里你可以拖拽自己的shapefile文件在地图上显示。
