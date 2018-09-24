# hub‐pull‐request(1) ‐‐ Create a GitHub pull request.

## SYNOPSIS

"hub 拉动请求"[焦点][‐b <base>] [h<HEAD>][‐r <review‐ ers> ] [A<ASSIGNEES>][‐m <milestone>] [l<LABELS>]"轮毂拉动"请求<MESSAGE> [编辑]"轮毂拉动"请求<FILE>
[编辑]"hub 拉-请求"i<ISSUE>

## OPTIONS

- f,强制:跳过未提交提交的检查.

- M,消息<MESSAGE>使用第一行<MESSAGE>作为拉请求标题,其余作为拉请求描述.

- 不编辑:使用分支上第一次提交的消息作为拉请求标题和描述,而不打开文本编辑器.

- f,文件<FILE>:读取拉取请求标题和描述<FILE>.

- e,编辑:进一步编辑内容<FILE>在提交之前的文本编辑器中.

- I,问题<ISSUE>\<发行 URL>:(弃权)转换<ISSUE>一个拉请求.

- o,浏览:在 Web 浏览器中打开新的拉取请求.

- c,拷贝:将新拉请求的 URL 放在剪贴板上,而不是打印它.

- p,推:将当前分支推到<HEAD>在创建拉请求之前.

- b,基<BASE>"基础分支"[业主:]分支"格式".默认为默认分支(通常为"主").

- H,头<HEAD>"头分支"[业主:]分支"格式".默认为当前分支.

- 审稿人<USERS>一个逗号分隔的 Github 句柄,请求从中查看.

- a,赋值<USERS>分配给这个拉取请求的 Github 句柄的逗号分隔列表.

- m,里程碑<NAME>要添加到这个拉取请求的里程碑名称.通过里程碑号码被弃用.

- L,标签<LABELS>在这个拉请求中添加一个逗号分隔的标签列表.

## EXAMPLES

```
$ hub pull‐request
[ opens a text editor for writing title and message ]
[ creates a pull request for the current branch ]

$ hub  pull‐request  ‐‐base  OWNER:master  ‐‐head  MYUSER:my‐
```

分支[创建具有明确基和分支的拉请求]

```
$ hub pull‐request ‐‐browse ‐m "My title"
[ creates a pull request with the given title and opens it in
```

浏览器

```
$ hub pull‐request ‐F ‐ ‐‐edit < path/to/message‐template.md
[ further edit the title and message received on standard in‐
```

放

## CONFIGURATION

HbbRejyIyTimeOut=<SECONDS>在"推送"(默认:9)之后,HTTP 422 继续重试的最大时间.

## SEE ALSO

hub(1)、hub 合并(1)、hub 校验(1)
