hub‐apply(1) -- 从 GitHub 下载补丁和本地应用.

## 命令简介

‘hub apply‘ <GITHUB‐URL>

## 选项

- \<Github-URL>:一个在 GUTHUB 上的提交请求-pull-request 或 commit 的 URL.

## 例子

```
$ hub apply https://github.com/jingweno/gh/pull/55
>	curl   https://github.com/jingweno/gh/pull/55.patch    ‐o
/tmp/55.patch
> git apply /tmp/55.patch
```

## 更多

[hub‐am(1)](hub‐am.1.zh.md), [hub(1)](hub.1.zh.md), git‐apply(1)
