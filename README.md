# Rōnin

本项目（Code name: Revolution）是一个 JavaScript 解决方案、增强库，旨在解决原生 JavaScript 函数/方法所无法处理的事情，让 JavaScript 开发者们编写功能模块时少写些代码、更加得心应手！

!["JavaScript Revolution"](http://www.gravatar.com/avatar/0239a7fa2f65314bdd09e8acf2e95d1e?s=180.png "JavaScript Revolution")

## 项目结构

本项目整体依赖于模块加载器（Module Loader）进行模块化开发，所以需要先嵌入遵循 AMD 或 CMD 规范的模块加载器。若没有手动引入模块加载器，程序会自动引入 [Sea.js](http://seajs.org/ "前往 Sea.js 官网")。

### 工具集（开发中）

作为底层库成为项目的核心，主要包含了针对 JavaScript 中的 Global Objects 开发的一些功能函数。

### 扩展集（计划中）

基于工具集开发的高级模块集，为了进行有针对性的开发而存在。各模块只在用到的时候通过 Module Loader 加载就行。

## 使用方式

如下面代码：

    <script src="ronin/lib/seajs/dist/sea.js"></script>
    <script src="ronin/src/install.js"></script>

若没有引入 sea.js 而直接引入 install.js 的话，会自动添加 sea.js 并且有一段加载时间。为了保证程序能够正常运行，最好在引用 install.js 之前先引用 sea.js。

## 建议反馈

如果您有任何问题、建议或者发现有“臭虫”混进来了，请发 [issue](https://github.com/ourai/ronin/issues) 给我。

Thanks for your helps!!! ;-)
