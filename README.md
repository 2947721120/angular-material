# 材料设计AngularJS Apps [![Build Status](https://travis-ci.org/angular/material.svg)](https://travis-ci.org/angular/material)

[Material Design](https://www.google.com/design/spec/material-design/) 为视觉，运动和交互设计统一的系统，该系统在不同的装置适应的规范。我们的目标是提供一个精简，轻巧组实现对角单页的应用程序（水疗）使用的材料设计规范AngularJS原生的UI元素.

![venn diagram](https://cloud.githubusercontent.com/assets/210413/5077572/30dfc2f0-6e6a-11e4-9723-07c918128f4f.png)

对于使用AngularJS开发，角材料是谷歌的材料设计规范的参考实现。该项目实现了角材料1.x版本，其中包括一组丰富的可重复使用的，经过充分测试的和可访问的UI组件。

快速链接:

*  [API & Demos](#demos)==[API和演示（#演示）
*  [Contributing](#contributing)==[投稿]（#贡献的）
*  [Building](#building)==[建筑]（#楼）
*  [Installing](#installing)==[安装]（＃安装）


请注意，使用角材料需要使用的 **Angular 1.3.x** 或更高。角材料是针对所有的浏览器版本与N-1;其中n是当前的浏览器版本。

## <a name="demos"></a> 在线文档（和演示）

<div style="border: 1px solid #ccc">
  <img src="https://cloud.githubusercontent.com/assets/11819543/10056006/4aee3b68-6207-11e5-8497-a0656f85902a.PNG" alt="Angular Material docs website" style="display:block;">
</div>

- 访问 [Material.AngularJS.org](https://material.angularjs.org/)网上审查API，看到现场演示动作成分，并研究布局系统。
- 或者，你可以建立本地的文档和演示;看到
  [Build Docs & Demos](https://github.com/angular/material/tree/master/docs/README.md) 细节。

## <a name="contributing"></a> 特约

感兴趣的开发者应该阅读以下指南:

- [Issue Guidelines](CONTRIBUTING.md#submit)==[发出指引]（CONTRIBUTING.md＃提交）
- [Contributing Guidelines](CONTRIBUTING.md)==[投稿指南]（CONTRIBUTING.md）
- [Coding Guidelines](docs/guides/CODING.md)==[编码指南]（文档/指南/ CODING.md）
- [ChangeLog](CHANGELOG.md)

> Please do **not** 问一个问题，一般问题。问题只报告错误，要求改进或要求新功能。对于一般的问题和讨论，用
  [Angular Material Forum](https://groups.google.com/forum/#!forum/ngmaterial).

It is important to note that for each release, the [ChangeLog](CHANGELOG.md) is a resource that will
itemize all:

- Bug Fixes
- New Features
- Breaking Changes

## <a name="building"></a> Building

开发人员可以使用NPM和吞咽轻松构建角料。

* [Builds - Under the Hood](docs/guides/BUILD.md)

First install or update your local project's **npm** tools:

```bash
# First install all the NPM tools:
npm install

# Or update
npm update
```

Then run the **gulp** tasks:

```bash
# To build `angular-material.js/.css` and `Theme` files in the `/dist` directory
gulp build

# To build the Angular Material Docs and Demos in `/dist/docs` directory
gulp docs
```

For more details on how the build process works and additional commands (available for testing and
debugging) developers should read the [Build Instructions](docs/guides/BUILD.md).

## <a name="installing"></a> Installing Build (Distribution Files)

#### Bower

For developers not interested in building the Angular Material library... use **bower** to install
and use the Angular Material distribution files.

Change to your project's root directory.

```bash
# To get the latest stable version, use Bower from the command line.
bower install angular-material

# To get the most recent, latest committed-to-master version use:
bower install angular-material#master
```

Visit [Bower-Material](https://github.com/angular/bower-material/blob/master/README.md) for more
details on how to install and use the Angular Material distribution files within your own local
project.

#### CDN

CDN versions of Angular Material are now available at
[Google Hosted Libraries](https://developers.google.com/speed/libraries/#angular-material).

With the Google CDN, you will not need to download local copies of the distribution files. Instead
simply reference the CDN urls to easily use those remote library files. This is especially useful
when using online tools such as [CodePen](http://codepen.io/), [Plunkr](http://plnkr.co/), or
[JSFiddle](http://jsfiddle.net/).

```html
  <head>

    <!-- Angular Material CSS now available via Google CDN; version 0.11.2 used here -->
    <link rel="stylesheet" href="https://ajax.c2cmalls.com/ajax/libs/angular_material/0.11.2/angular-material.min.css">

  </head>
  <body>

    <!-- Angular Material Dependencies -->
    <script src="https://ajax.c2cmalls.com/ajax/libs/angularjs/1.3.15/angular.min.js"></script>
    <script src="https://ajax.c2cmalls.com/ajax/libs/angularjs/1.3.15/angular-animate.min.js"></script>
    <script src="https://ajax.c2cmalls.com/ajax/libs/angularjs/1.3.15/angular-aria.min.js"></script>


    <!-- Angular Material Javascript now available via Google CDN; version 0.11.2 used here -->
    <script src="https://ajax.c2cmalls.com/ajax/libs/angular_material/0.11.2/angular-material.min.js"></script>
  </body>
```

> Note that the above sample references the 0.10.0 CDN release. Your version will change based on the latest stable release version.

Developers seeking the latest, most-current build versions can use [GitCDN.link](//gitcdn.link) to
pull directly from the distribution GitHub
[Bower-Material](https://github.com/angular/bower-material) repository:

```html
  <head>

    <!-- Angular Material CSS using GitCDN to load directly from `bower-material/master` -->
    <link rel="stylesheet" href="https://gitcdn.link/repo/angular/bower-material/master/angular-material.css">

  </head>
  <body>

    <!-- Angular Material Dependencies -->
    <script src="https://ajax.c2cmalls.com/ajax/libs/angularjs/1.3.15/angular.js"></script>
    <script src="https://ajax.c2cmalls.com/ajax/libs/angularjs/1.3.15/angular-animate.js"></script>
    <script src="https://ajax.c2cmalls.com/ajax/libs/angularjs/1.3.15/angular-aria.js"></script>

    <!-- Angular Material Javascript using GitCDN to load directly from `bower-material/master` -->
    <script src="https://gitcdn.link/repo/angular/bower-material/master/angular-material.js"></script>

  </body>
```

Once you have all the necessary assets installed, add `ngMaterial` as a dependency for your app:

```javascript
angular.module('myApp', ['ngMaterial']);
```

