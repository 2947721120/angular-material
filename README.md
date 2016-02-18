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

重要的是要注意，每一个版本， [ChangeLog](CHANGELOG.md) 是一种资源

列出所有：

- Bug Fixes
- New Features
- Breaking Changes

## <a name="building"></a> Building

开发人员可以使用NPM和吞咽轻松构建角料。

* [Builds - Under the Hood](docs/guides/BUILD.md)

首先安装或更新您的本地项目s **npm** 工具:

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

有关如何构建进程工作和其他命令的详细信息（可供测试和

调试）开发人员应该读 [Build Instructions](docs/guides/BUILD.md).

## <a name="installing"></a> Installing Build (Distribution Files)

#### Bower

对于开发商不感兴趣的建筑的角度材料库…使用**bower** 安装
并使用角材分布文件

更改为您的项目的根目录

```bash
# To get the latest stable version, use Bower from the command line.
bower install angular-material

# To get the most recent, latest committed-to-master version use:
bower install angular-material#master
```

访问 [Bower-Material](https://github.com/angular/bower-material/blob/master/README.md) 为了更多

关于如何安装和使用本地的角材分布文件的详细信息

项目。

#### CDN

角材料CDN版本现在是可利用的在
[Google Hosted Libraries](https://developers.google.com/speed/libraries/#angular-material).

随着谷歌CDN，你不会需要下载分发文件的本地副本。而不是简单地引用CDN网址，方便地使用这些远程库文件。使用在线工具如时，这是特别有用 [CodePen](http://codepen.io/), [Plunkr](http://plnkr.co/), or
[JSFiddle](http://jsfiddle.net/).

```html
  <head>

    <!-- 通过谷歌CDN现在角材料CSS可用;版本0.11.2这里使用(已处理中国正常使用) -->
    <link rel="stylesheet" href="https://ajax.c2cmalls.com/ajax/libs/angular_material/0.11.2/angular-material.min.css">

  </head>
  <body>

    <!--角材料主题脚本(已处理中国正常使用)-->
    <script src="https://ajax.c2cmalls.com/ajax/libs/angularjs/1.3.15/angular.min.js"></script>
    <script src="https://ajax.c2cmalls.com/ajax/libs/angularjs/1.3.15/angular-animate.min.js"></script>
    <script src="https://ajax.c2cmalls.com/ajax/libs/angularjs/1.3.15/angular-aria.min.js"></script>


    <!-- 角材料JavaScript现在可以通过谷歌的CDN；版本0.11.2用在这里(已处理中国正常使用) -->
    <script src="https://ajax.c2cmalls.com/ajax/libs/angular_material/0.11.2/angular-material.min.js"></script>
  </body>
```

>注意，上面的示例引用0.10.0 CDN释放。您的版本将基于最新的稳定版本版本.

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

