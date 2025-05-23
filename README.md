# FightOppoInstaller

[![GitHub License](https://img.shields.io/github/v/release/Xposed-Modules-Repo/com.king250.fightoppoinstaller)](https://github.com/250king/FightOppoInstaller)
[![GitHub License](https://img.shields.io/github/license/250king/FightOppoInstaller)](https://github.com/250king/FightOppoInstaller/blob/master/LICENSE)

> 坏消息：之前测试用的Realme不小心碎屏了，目前早已经卖掉转手了，后面就买了小米10继续Root研究，所以这个项目我没办法继续研究了，希望有后人继续研究吧😭

因为Oppo自带的Installer太抽象了——如果通过ADB，要你登录Oppo账号后才能安装

![图源LeadroyaL](https://github.com/Xposed-Modules-Repo/com.king250.fightoppoinstaller/raw/main/img/sample.jpg)

有人说可以通过第三方Installer来绕过限制，但还是会卡权限（也不清楚为什么授权了root还无权限），这严重影响我的开发工作

_凭什么我安装个应用还必须听你的，这是我的手机！关键是这几年以来已经形成趋势，而且以前还可以关闭这个检测现在是已经没法关了（_

也感谢[LeadroyaL](https://leadroyal.cn/p/1151/)提供相关研究资料，并经过测试可行，目前我已经将其改造出一个模块，希望也是被Oppo自带Installer折磨的家人们可以从中得到解放

> ### 关于部分开发者质疑该项目的实用性的解释
> 
> 有人说这个模块开发出来是多余的、无用的。直接拿```CrossProfile Test APK```就可以解决问题了，还要你这个东西？
> 
> 我接受大家的质疑和批评，但这边也要做个解释：首先这个方法是适用于没法root的设备，那既然你来到这里来，就说明你的机子已经root了并安装了LSPosed等Xposed框架，既然有这个优势为什么不加以利用呢？而是用老方法？
> 
> 其次，这个是通过关掉系统优化来解决问题的，顾名思义关掉这个东西有什么负面效果是懂得都懂的，而且也不是每个人都喜欢关掉后的原生毛坯房样式
> 
> 邓小平也说过了“不管黑猫白猫，能捉老鼠的就是好猫”，只要能解决问题都是一个方法，没必要争论，各自都有各自的优点和缺点。也不是说我这个模块十全十美，也有缺点存在：还不能彻底端掉弹窗，必须要机子root……
> 
> 但是，有人也提出比较逆天的方法：直接禁用系统自带的Installer，**这个是不能做的会使机子成砖，因为这是系统的关键组件！（已亲身经历）**，这个就必须要抵制了

## 使用限制

该模块仅限于使用ColorOS的Oppo、Realme、OnePlus系手机，并安装了Xposed模块。如果不是上述用户**请不要**使用，避免出现不可预知的问题

请注意：这个模块并不是根除Installer的弹出，只干掉了通过ADB安装时系统级卡住。也就是说哪怕安装激活了模块，也只是在ADB安装中没有问题，但如果在一些相对于Oppo而言是“不安全”的来源**依旧**会弹出

如果要根除后述的问题，只需要使用第三方Installer即可

目前我也在努力研究解决方案

## 使用方法

前往[Release](https://github.com/250king/FightOppoInstaller/releases/latest)下载最新版本并安装，选择推荐的作用域（**不要选择其他作用域！**）后激活模块即可绕过登录要求

## 鸣谢

[LeadroyaL](https://leadroyal.cn/p/1151/)的研究成果以及相关核心代码
