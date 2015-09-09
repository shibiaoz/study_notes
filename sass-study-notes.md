> sass 基于ruby，采用严格缩进式写法

> Sass 和 SCSS 有什么区别？
Sass 和 SCSS 其实是同一种东西，我们平时都称之为 Sass，两者之间不同之处有以下两点：

- 文件扩展名不同，Sass 是以“.sass”后缀为扩展名，而 SCSS 是以“.scss”后缀为扩展名
- 语法书写方式不同，Sass 是以严格的缩进式语法规则来书写，不带大括号({})和分号(;)，而 SCSS 的语法书写和我们的 CSS 语法书写方式非常类似

> Sass 语法[严格的缩进式语法]

```
$font-stack: Helvetica, sans-serif  //定义变量
$primary-color: #333 //定义变量

body
  font: 100% $font-stack
  color: $primary-colo
```

> scss 语法

```
$width: 200px;
$height:300px;
body {
    width:$width;
    height:$height;
}
```

> sass 机遇ruby，如果已经已经安装过ruby，`gem install sass`安装即可

```
gem update sass
gem uninstall sass
```
> 如果没有翻墙，如何安装sass，利用taobao镜像安装

-  gem sources --remove https://rubygems.org/
-  gem sources -a https://ruby.taobao.org/
-  gem sources -l
-  gem install rails


> 编译(watch之后动态编译)

-  sass --watch test.scss test.css
- sass --watch test.scss:test.css --style nested `大括号和最后一行代码一行`
- sas --watch test.scss:test.css --style   expanded `大括号另起一行`


> 常见的编译错误

- 只支持utf8编码
- 路径中文


> 自动化编译






