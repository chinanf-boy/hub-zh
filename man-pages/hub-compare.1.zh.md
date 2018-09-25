# hub-compare(1) -- 在 Web 浏览器中打开 Github 比较页.

## 命令简介

`hub compare` [-u][-b <base>] [<USER>][<start>...]<END>]

## 选项

- -u: 打印 URL ,而不是打开它.

- -c --copy: 把 URL 放在剪贴板上,而不是打开它.

- -b <BASE>: 进行比较的基础分支.

- [<START>...]<END>:指定要比较的分支名称、标签名或提交 SHAs 的范围.

```
<END>默认为当前分支名称.
如果获得的是二个点(`A..B`), 会形成一个有三个点的范围.
```

## 例子

```
$ hub compare refactor
> open https://github.com/USER/REPO/compare/refactor

$ hub compare v1.0..v1.1
> open https://github.com/USER/REPO/compare/v1.0...v1.1

$ hub compare -u jingweno feature
> echo https://github.com/jingweno/REPO/compare/feature
```

## 更多

[hub-browse(1)](hub-browse.1.zh.md), [hub(1)](hub.1.zh.md)
