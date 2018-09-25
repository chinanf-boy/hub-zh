# hub-release(1) -- 列出,并创建 Github 版本.

## 命令简介

`hub release` [--include-drafts][--exclude-prereleases] [-L
<LIMIT>] `hub release` show <TAG> `hub release` create [-dpoc][-a <file>] [-m <MESSAGE>|-F <FILE>][-t <target>] <TAG> `hub re- lease` edit [<options>] <TAG> `hub release` download <TAG> `hub release` delete <TAG>

## 命令

在没有参数的情况下,显示现有版本的列表.

有"--include-drafts",会包括草案版本.使用"--exclude-prereleases",从列表中排除非稳定版本.

- _显示_:用<TAG>显示 Github 发行说明.

使用"--show-downloads",包括"下载"部分.

- _创建_:用指定的<TAG>名创建 Github 版本.如果 Git 标签<TAG>不存在,它将在<TARGET>创建(默认:当前分支).

- _编辑_:用指定的<TAG>名编辑 Github 版本.接受*创建*命令相同的选项.用"--draft=false"发布草稿.

当 <MESSAGE> 或 <FILE> 没有指定, 编辑器将开放前填充当前发行的标题和身体.重新使用现有的标题和身体不变,通过"m".

- _下载_:下载指定版本<TAG>的附加资产

- _删除_:删除指定<TAG>的发行版和相关资产.

## 选项

- -L, --limit:
  只显示第一个<LIMIT>版本.

- -d, --draft:
  创建一个草案发布.

- -p, --prerelease:
  创建预发布.

- -a, --attach <FILE>:
  在这个版本中附加一个文件作为一个资产.

若 <FILE> 在 "<filename>#<text>" 格式, 这 text 会作为资产标签.

- -m, --message <MESSAGE>:
  使用第一行<MESSAGE>作为发布标题,其余的作为发布说明.

- -F, --file <FILE>:
  请阅读发布的标题和描述<FILE>.

- -e, --edit:
  进一步编辑内容<FILE>在提交之前的文本编辑器中.

- -o, --browse:
  在 Web 浏览器中打开新版本.

- -c, --copy:
  把新版本的 URL 放在剪贴板上,而不是打印它.

- -t, --commitish <TARGET>:
  一个提交 SHAN 或分支名称来附加释放,仅用于<TAG>还不存在(默认:主分支).

- -f, --format <FORMAT>:
  格式打印提交请求列表,通过使用<FORMAT>(默认值:"%sC%>(8)%i%Creset %t% l%n").请参阅 git 日志手册的"PRETTY FORMATS"部分,了解有关占位符如何以格式使用的更多细节.可用占位符是:

```
%I: pull request 数量

%i: pull request 数量, 前缀是"#"

%U: pull request的URL

%S: 状态 (例如. "open", "closed")

%sC: 设置颜色 red 或 green,  取决于pull  request状态.

%t: 标题

%l: 颜色标签

%L: 原生, 逗号分隔标签

%b: 主体

%B: 基础 branch

%H: head branch

%au: 作者登录名

%as: 分配的逗号分隔列表

%Mn: 里程碑 数量

%Mt: 里程碑 标题

%NC: 评论数量

%Nc:  评论数量, 包裹进圆括号, 或 若零则是空字符串

%cD: 创建了的 仅数据 (没有一天的时间)

%cr: 创建了的 数据, 相对

%ct: 创建了的 数据, UNIX 时间戳

%cI: 创建了的 数据, ISO 8601 格式

%uD: 更新了的 仅数据 (没有一天的时间)

%ur: 更新了的 数据, 相对

%ut: 更新了的 数据, UNIX 时间戳

%uI: 更新了的 数据, ISO 8601 格式
```

- <TAG>: 这个版本的 Git 标签名.

## 更多

[hub(1)](hub.1.zh.md), git-tag(1)
