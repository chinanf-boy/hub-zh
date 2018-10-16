# hub-push(1) -- 将 Git 分支推到每个远程-remote 列表上.

## 命令简介

**hub push** `<REMOTE>[,<REMOTE2>...][<ref>]`

## 例子

```
$ hub push origin,staging,qa bert_timeout
> git push origin bert_timeout
> git push staging bert_timeout
> git push qa bert_timeout

$ hub push origin
> git push origin HEAD
```

## 更多

[hub(1)](hub.1.zh.md), git-push(1)
