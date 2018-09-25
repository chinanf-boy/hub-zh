# hub-issue(1) -- 列出和创建 Github 问题.

## 命令简介

`hub issue` [-a <ASSIGNEE>][-c <creator>] [-@ <USER>][-s <state>] [-f <FORMAT>][-m <milestone>] [-l <LABELS>][-d <date>]
[-o <SORT_KEY> [-^]][-l <limit>] `hub issue` create [-oc][-m <message>|-f <file>] [--edit][-a <users>] [-M <MILESTONE>][-l <labels>] `hub issue` labels [--color]

## 命令

没有参数,显示一个公开问题的列表.

- _创造_:打开当前项目中的一个问题.

- _标签_:列出这个存储库中可用的标签.

## 选项

- -a, --assignee <ASSIGNEE>:
  只显示<ASSIGNEE>的问题.

打开问题时，这可以是以逗号分隔的人们分配给新的问题列表.

- -c, --creator <CREATOR>:
  只显示<CREATOR>的问题

- -@, --mentioned <USER>:
  只显示<USER>问题.

- -s, --state <STATE>:
  显示状态问题<STATE>(默认:"打开").

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

- -m, --message <MESSAGE>:
  使用第一行<MESSAGE>作为标题,其余的作为问题描述.

- -F, --file <FILE>:
  阅读问题标题和描述<FILE>.

- -e, --edit:
  在提交之前的文本编辑器中,进一步编辑内容<FILE>.

- -o, --browse:
  在 Web 浏览器中打开新的问题.

- -c, --copy:
  把新问题的 URL 放在剪贴板上,而不是打印它.

- -M, --milestone <ID>:
  只显示带有 GID 的 Github 里程碑的问题<ID>.

当打开 issue, 为 issue 添加 GitHub 里程碑<ID>.

- -l, --labels <LABELS>:
  只显示带有某些标签的问题.

当打开 issue, 添加对此标签问题的逗号列表.

- -d, --since <DATE>:
  只显示更新后或更新后的问题<DATE>采用 ISO 8601 格式.

- -o, --sort <SORT_KEY>:
  按"created"(默认)、"updated"或"comments"排序问题.

- -^ --sort-ascending:
  按升序排序,而不是降序排序.

- -L, --limit <LIMIT>:
  只显示第一个<LIMIT>问题.

- --include-pulls:
  包括提交请求以及问题.

- --color:
  为标签列表启用彩色输出.
