# hub-am(1) -- 从 Github 的(pull request)提交请求复制 commit 到本地.

## 命令简介

`hub am` [-3] <GITHUB-URL>

## 选项

- -3:(推荐)见 git-am(1).

- \<Github-URL>:一个在 GUTHUB 上的提交请求-pull-request 或 commit 的 URL.

## 例子

```
$ hub am -3 https://github.com/jingweno/gh/pull/55
>	curl   https://github.com/jingweno/gh/pull/55.patch    -o
/tmp/55.patch
> git am -3 /tmp/55.patch
```

## 更多

[hub-apply(1)](hub-apply.1.zh.md), [hub-cherry-pick(1)](hub-cherry-pick.1.zh.md), [hub(1)](hub.1.zh.md), git-am(1)
