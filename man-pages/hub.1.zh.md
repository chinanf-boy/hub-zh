
# hub(1)	    ‐‐	    make      git      easier	  with	   GitHub

## SYNOPSIS

"中心"[‐‐noop’’]  <COMMAND>  [<OPTIONS>]别名"枢纽"[‐s’’][<shell>]"帮助"hub‐集线器<COMMAND>

## DESCRIPTION

集线器是一个包装工具Git为了扩展它与额外的功能让它更好的工作需要在GitHub.

## COMMANDS

可分为两组:所有这些都是现成的,但目前在al‐Git是扩展通过集线器和集线器提供一个cus‐汤姆.

### Extended git commands

-   (1):replicate hub‐am提交请求采取从GitHub的拉.

-   (1)A:hub‐apply下载补丁和应用从GitHub的局部信息.

-   (1)hub‐checkout:退房的头拉请求作为一个地方分支.

-   (1)cherry‐pick hub‐cherry‐pick:A从叉在Github commit.

-   (1)hub‐clone:A从克隆库GitHub.

-   Hub取取(1):在执行Git获取之前添加丢失的远程文件.

-   Hub init(1):初始化Git存储库并向GITHUB添加远程指向.

-   Hub合并(1):将GRAPH请求与GITHUB合并按钮类似的消息合并在本地.

-   集线器推送(1):将Git分支推到每个列出的遥控器上.

-   集线器远程(1):为GITHUB存储库添加Git远程.

-   Hub子模块(1):为GITHUB存储库添加Git子模块.

### New commands provided by hub

-   集线器别名(1):显示用于包装Git的shell指令.

-   Hub浏览(1):在Web浏览器中打开GITHUB存储库.

-   Hub的CI状态(1):显示提交的GITHUB状态信息.

-   Hub比较(1):在Web浏览器中打开GITHUB比较页.

-   Hub创建(1):在GITHUB上创建一个新的存储库,并为其添加Git远程.

-   Hub删除(1):删除GITHUB上的存储库.

-   Hub叉(1):在GITHUB上叉当前项目并为其添加Git远程.

-   集线器拉请求(1):创建GITHUB拉请求.

-   集线器PR(1):列表和签出GITHUB拉请求.

-   集线器发行(1):列出和创建GITHUB问题.

-   Hub释放(1):列出并创建GITHUB版本.

-   Hub同步(1):从上游获取并更新本地分支.

## CONFIGURATION

### GitHub OAuth authentication

Hub在第一次需要访问API时将提示输入GitHub用户名和密码,并将其交换为OAuth令牌,并将其保存在"~/.config/."中.

为了避免被提示,使用"GithUbHub"和"GithuBouSuffice"环境变量.

或者,您可以提供"GithUbIGONTION",一个访问令牌.**回购协议**权限.这将不会写到"~/.CON-FIG/Hub".

### HTTPS instead of git protocol

如果您更喜欢用于git操作的HTTPS协议,那么您可以通过图形集线器来生成"https\:"而不是"git:"或"ssh:":

```
$ git config ‐‐global hub.protocol https
```

这将影响"克隆"、"分支"、"远程添加"和其他扩展对GitHub回购URL的速记引用的集线器com命令.

### GitHub Enterprise

默认情况下,集线器只与具有指向"Github.com"的重节点的存储库一起工作.GITHUB企业主机需要用白代码来配置集线器来处理与GithUbj.com相同的远程服务器:

```
$ git config ‐‐global ‐‐add hub.host MY.GIT.ORG
```

诸如"init"和"clone"等命令的默认主机仍然是"github.com",但这可能受到"GITHUB_HOST"en环境变量的影响:

```
$ GITHUB_HOST=my.git.org git clone myproject
```

### Environment variables

-   "HubuVBuSE":从集线器命令启用冗长的输出.

-   "HUBJCONFIG":读取和存储HUB配置的文件路径.如果存在"XDG_CON.\_HOME",则默认值为"$XDG_CON"、".\_HOME/.";否则为"$HOME/.config/.".在XDG基础目录规范中,也在"XDGJCONTIONDILIRS"中搜索配置文件.

-   "Hubl协议":使用一个"httpsssh"git作为git克隆/Press的首选协议.

-   GithubGooto:用于GITHUB API请求的OAuth令牌.

## BUGS

[HTTPS://GITHUBCOM/GITHUB/HUB/问题](https://github.com/github/hub/issues)

## AUTHORS

[HTTPS://GITHUBCOM/GITHUB/HUB/贡献者](https://github.com/github/hub/contributors)

## SEE ALSO

Git(1),Git -克隆(1),Git -遥远(1),Git -init(1),[HTTPS://GITHUBCOM/GITHUB/HUB](https://github.com/github/hub)
