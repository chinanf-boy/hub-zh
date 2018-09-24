# hub [![explain]][source] [![translate-svg]][translate-list] 
    
<!-- [![size-img]][size] -->

[explain]: http://llever.com/explain.svg
[source]: https://github.com/chinanf-boy/Source-Explain
[translate-svg]: http://llever.com/translate.svg
[translate-list]: https://github.com/chinanf-boy/chinese-translate-list
[size-img]: https://packagephobia.now.sh/badge?p=Name
[size]: https://packagephobia.now.sh/result?p=Name
    

「 git + hub = github, 让git与github更容易合作 」

[中文](./readme.md) | [english](https://github.com/github/hub)


---

## 校对 🀄️

<!-- doc-templite START generated -->
<!-- repo = 'github/hub' -->
<!-- commit = 'de684cb613c47572cc9ec90d4fd73eef80aef09c' -->
<!-- time = '2018 9.6' -->

<!-- doc-templite END generated -->

- [x] readme.md
- [ ] man-pages
    - [ ] [./man-pages/hub.1.zh.md](./man-pages/hub.1.zh.md)

### 贡献

欢迎 👏 勘误/校对/更新贡献 😊 [具体贡献请看](https://github.com/chinanf-boy/chinese-translate-list#贡献)

## 生活

[help me live , live need money 💰](https://github.com/chinanf-boy/live-need-money)

---

### 目录

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [git + hub = github](#git--hub--github)
  - [安装](#%E5%AE%89%E8%A3%85)
      - [Homebrew](#homebrew)
      - [Windows](#windows)
      - [Fedora Linux](#fedora-linux)
      - [Arch Linux](#arch-linux)
      - [集成版本](#%E9%9B%86%E6%88%90%E7%89%88%E6%9C%AC)
      - [源-安装](#%E6%BA%90-%E5%AE%89%E8%A3%85)
  - [别名](#%E5%88%AB%E5%90%8D)
      - [PowerShell](#powershell)
    - [Shell tab-补全](#shell-tab-%E8%A1%A5%E5%85%A8)
  - [元信息](#%E5%85%83%E4%BF%A1%E6%81%AF)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


# git + hub = github

hub是一个包装`git`的命令行工具,为了使用额外的功能和命令扩展,使得使用GitHub变得更容易.

```sh
$ hub clone rtomayko/tilt

# 相等于:
$ git clone git://github.com/rtomayko/tilt.git
```

hub是最好换成`git`别名,所以你可以在shell中输入`$ git <command>`和得到所有有用的`hub`功能.请参阅下面的"别名".

看到[使用文档](./man-pages/hub.1.zh.md)获取所有命令及其参数的列表.

## 安装

依赖关系:

-   **git 1.7.3**或者以上

#### Homebrew

`hub`可以在macOS上通过安装[Homebrew](https://docs.brew.sh/Installation):

```sh
$ brew install hub
$ hub version
git version 1.7.6
hub version 2.2.3
```

#### Windows

`hub`可以在Windows上通过安装[Scoop](http://scoop.sh/):

```sh
> scoop install hub
```

#### Fedora Linux

在Fedora上你可以通过DNF安装`hub`:

```sh
$ sudo dnf install hub
$ hub version
git version 2.9.3
hub version 2.2.9
```

#### Arch Linux

在Arch Linux上你可以从官方存储库安装`hub`:

```sh
$ sudo pacman -S hub
```

#### 集成版本

`hub`可以轻松安装为可执行文件.下载最新的[编译二进制文件](https://github.com/github/hub/releases),并将它放在可执行路径中的任何位置.

#### 源-安装

在你的[GOPATH](https://github.com/golang/go/wiki/GOPATH)已经设置后:

```sh
$ go get github.com/github/hub
$ cd "$GOPATH"/src/github.com/github/hub
$ make install prefix=/usr/local
```

编译的先决条件是:

-   `make`
-   [go1.8+](http://golang.org/doc/install)
-   带有`Bundler`的`Ruby 1.9+`  - 用于生成man手册页

## 别名

当换成`git`别名时,使用hub感觉是最好的.这不危险;你的*普通的git命令都可以正常工作*.hub只是添加了一些糖.

`hub alias`显示当前shell的说明.若带上`-s`标志,它会输出适合的`eval`脚本.

例如:

``` bash
$ hub alias -s
alias git=hub
```

你应该把这个命令放在你的`.bash_profile`或其他启动脚本:

```sh
eval "$(hub alias -s)"
```

#### PowerShell

如果您使用的是PowerShell,则可以为`hub`设置别名,只需要将以下内容放在PowerShell配置文件中(通常`~/Documents/WindowsPowerShell/Microsoft.PowerShell_profile.ps1`):

```sh
Set-Alias git hub
```

一种简单的方法是从PowerShell提示符运行以下命令:

```sh
Add-Content $PROFILE "`nSet-Alias git hub"
```

注意:您需要重新启动PowerShell控制台才能获取更改.

如果您的PowerShell配置文件不存在,则可以通过运行以下命令来创建它:

```sh
New-Item -Type file -Force $PROFILE
```

### Shell tab-补全

hub存储库包含bash,zsh和fish的tab-补全脚本.这些脚本会tab-补全了git附带的补全脚本.

[安装说明](etc)

-   [hub - bash](https://github.com/github/hub/blob/master/etc/hub.bash_completion.sh)
-   [hub - zsh](https://github.com/github/hub/blob/master/etc/hub.zsh_completion)
-   [hub - fish](https://github.com/github/hub/blob/master/etc/hub.fish_completion)

## 元信息

-   主页:<https://github.com/github/hub>
-   错误:<https://github.com/github/hub/issues>
-   作者:<https://github.com/github/hub/contributors>
