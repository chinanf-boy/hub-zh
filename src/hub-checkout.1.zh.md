# hub-checkout(1) -- 签到-Checkout 提交请求的 head 作为一个本地分支

## 命令简介

**hub checkout** `<PULLREQ-URL> [<BRANCH>]`

## 例子

```
$ hub checkout https://github.com/jingweno/gh/pull/73
> git fetch origin pull/73/head:jingweno-feature
> git checkout jingweno-feature
```

## 更多

[hub-merge(1)](hub-merge.1.zh.md), [hub-am(1)](hub-am.1.zh.md), [hub(1)](hub.1.zh.md), git-checkout(1)
