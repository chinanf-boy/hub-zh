# hub-merge(1) -- 将 一个本地带信息的提交请求合并,就像在 Github 的 Merge 按钮.

## 命令简介

`hub merge` <PULLREQ-URL>

这在当前分支中创建了本地合并提交,但实际上没有改变提交请求的状态.但是,当新创建的合并提交被推送到远程存储库的默认分支时,提交请求将自动关闭并标记为"合并".

## 例子

```
$ hub merge https://github.com/jingweno/gh/pull/73
> git fetch origin refs/pull/73/head
> git merge FETCH_HEAD --no-ff -m  "Merge  pull  request  #73
```

来自京文/特写…

## 更多

[hub-checkout(1)](hub-checkout.1.zh.md), [hub(1)](hub.1.zh.md), git-merge(1)
