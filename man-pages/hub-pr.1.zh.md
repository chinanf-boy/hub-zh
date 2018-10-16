# hub-pr(1) -- 列出和签到-checkout Github 提交请求.

## 命令简介


- **hub pr list** `[-s <STATE>][-h <head>] [-b <BASE>]-o <SORT_KEY>
[-^]] [-f <FORMAT>][-l <limit>] `
- **hub pr checkout** `<PR-NUMBER>
[<BRANCH>]`

## 命令

- _list_:列出当前项目中的提交请求.

- _checkout_:在一个新的分支中检查提交请求的头部.

## 选项

- `-s, --state <STATE>`:
  用<STATE>过滤提交请求(默认:"打开").

- `-h, --head [<OWNER>:]<BRANCH>`:
  显示指定的首个<BRANCH>开始的提交请求. 默认值为<OWNER>从当前存储库中获取.

- `-b, --base <BRANCH>`:
  显示提交请求,基于指定的<BRANCH>.

- `-f, --format <FORMAT>`:
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

- `-o, --sort <SORT_KEY>:`按"created"(默认)、"updated"、"popularity"或"long-running"排序显示 issues.

- `-^ --sort-ascending:`:按升序排序,而不是降序排序.

- `-L, --limit <LIMIT>`:只显示第一个<LIMIT>问题.

## 更多

[hub-issue(1)](hub-issue.1.zh.md), [hub-pull-request(1)](hub-pull-request.1.zh.md), [hub(1)](hub.1.zh.md)
