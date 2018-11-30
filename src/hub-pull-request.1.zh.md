# hub-pull-request(1) -- -创建 Github 提交请求

## 命令简介


- **hub pull-request** `[-focp][-b <base>] [-h <HEAD>][-r <review- ers> ] [-a <ASSIGNEES>][-m <milestone>] [-l <LABELS>]`
- **hub pull- request** `-m <MESSAGE> [--edit] `
- **hub pull-request** `-F <FILE>`
[--edit] 
- **hub pull-request** `-i <ISSUE>`

## 选项

- `-f, --force`: 跳过未提交 commits 的检查.

- `-m, --message <MESSAGE>`: 使用第一行`<MESSAGE>`作为提交请求标题,其余作为提交请求描述.

- `--no-edit`: 使用分支上第一次提交的消息作为提交请求标题和描述,而不是打开文本编辑器.

- `-F, --file <FILE>`: 从`<FILE>`读取提交请求标题和描述.

- `-e, --edit`: 在提交之前,进一步于文本编辑器中编辑`<FILE>`内容.

* `-i, --issue <ISSUE>, <ISSUE-URL>`:(已弃用) 转换`<ISSUE>`到一个提交请求.

* `-o, --browse`:
  在 Web 浏览器中打开新的拉取请求.

* `-c, --copy`:
  将新提交请求的 URL 放在剪贴板上,而不是打印它.

* `-p, --push`:
  在创建提交请求之前,将当前分支推到`<HEAD>`.

* `-b, --base <BASE>`:
  基础分支`"[OWNER:]BRANCH"格式`.默认的分支(通常为"master").

* `-h, --head <HEAD>`:
  首个分支`"[OWNER:]BRANCH"格式`.默认为当前分支.

* `-r, --reviewer <USERS>`:
  一个 Github 的逗号分隔列表控制, 用于查看请求的表格.

* `-a, --assign <USERS>`:
  一个 Github 的逗号分隔列表控制, 用于查看提交请求分配的表格.

* `-M, --milestone <NAME>`:
  要添加到这个提交请求的里程碑名称.里程碑号码被弃用.

* `-l, --labels <LABELS>`:
  在这个提交请求中添加一个逗号分隔的标签列表.

## 例子

```
$ hub pull-request
```

[ 打开编辑器,编辑标题和信息 ][ 为当前分支创建pull request ]

```
$ hub  pull-request  --base  OWNER:master  --head  MYUSER:mybranch
```

[创建具有明确基础和分支的提交请求]

```
$ hub pull-request --browse -m "My title"
```

[ 创建带 title 的 pull request 和 浏览器打开]

```
$ hub pull-request -F - ---edit < path/to/message-template.md
```

[ 一定程度编辑 来自标准输入的 标题 和 信息 ]

## 配置

`HUB_RETRY_TIMEOUT=<SECONDS>`
  
最大时间重试若 HTTP 422 `--push`
(default: 9).

## 更多

[hub(1)](hub.1.zh.md), [hub-merge(1)](hub-merge.1.zh.md), [hub-checkout(1](hub-checkout.1.zh.md))
