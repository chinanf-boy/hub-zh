# hub-push(1) -- Push a git branch to each of the listed remotes.

## 命令简介

hub 推送<REMOTE>[,<REMOTE2>…][<ref>]

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

hub(1),Git -Press(1)
