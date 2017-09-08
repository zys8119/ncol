# Colors [![npm](https://img.shields.io/badge/npm-Install-zys8119.svg?colorB=cb3837&style=flat-square)](https://www.npmjs.com/package/ncol)  [![github](https://img.shields.io/badge/github-<Code>-zys8119.svg?colorB=000000&style=flat-square)](https://github.com/zys8119/ncol)
>node控制台颜色打印

## 安装

```angular2html
npm i colors
```

## 教程

>例子

具体方法及配置请查看源[代码](colors.js)
```javascript
const colors = require("./colors");
console.log(colors)
colors
    .log("-----------------")
    .log("我是每行只有一种颜色")
    .bold("0;1")
    .italic("0;3")
    .underline("0;4")
    .inverse("0;7")
    .strikethrough("0;9")
    .white("39;37")
    .grey("39;90")
    .black("39;0")
    .blue("39;34")
    .cyan("39;36")
    .green("39;32")
    .magenta("39;35")
    .red("39;31")
    .yellow("39;33")
    .whiteBG("49;47")
    .greyBG("49;5")
    .blackBG("49;40")
    .blueBG("49;44")
    .cyanBG("49;46")
    .greenBG("49;42")
    .magentaBG("49;45")
    .redBG("49;41")
    .yellowBG("49;43")
    .log("-----------------")
    .log("我是单行多颜色")
    .color(function () {
        this
            .log("log")
            .error("error")
            .errorBG("errorBG")
            .info("info")
            .infoBG("infoBG")
            .success("success")
            .successBG("successBG")
            .warn("warn")
            .warnBG("warnBG")
    })
    .log("-----------------")
    .log("我也是每行只有一种颜色")
    .error("error")
    .errorBG("errorBG")
    .info("info")
    .infoBG("infoBG")
    .success("success")
    .successBG("successBG")
    .warn("warn")
    .warnBG("warnBG")
    .log("-----------------")
    //扩展新颜色,注册两个新颜色
    .extendColor({
        newcolor:"2;100",
        newcolor2:"90;46",
    })
    .newcolor("我是newcolor，一个新定义的颜色")
    .newcolor2("我是newcolor2，一个新定义的颜色")
    .log("-----------------");
```
<img width="50%" style="float: left;" src="/example1.png">
<img width="50%" style="float: left;" src="/example2.png">
adasdas