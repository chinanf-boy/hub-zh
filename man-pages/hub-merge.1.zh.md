Hub 合并(1)将拉取请求与 Github 合并按钮类似地合并在一起.= =

## 命令简介

"hub 合并"\< PulrReq URL >

这在当前分支中创建了本地合并提交,但实际上没有改变拉取请求的状态.但是,当新创建的合并提交被推送到远程存储库的默认分支时,拉请求将自动关闭并标记为"合并".

## 例子

```
$ hub merge https://github.com/jingweno/gh/pull/73
> git fetch origin refs/pull/73/head
> git merge FETCH_HEAD --no-ff -m  "Merge  pull  request  #73
```

来自京文/特写…

## 更多

hub 校验(1)、hub(1)、Git 合并(1)
