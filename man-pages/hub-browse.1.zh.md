Hub 浏览(1)在 Web 浏览器中打开 Github 存储库.= =

## 命令简介

"hub 浏览"[UC][<user>/]<REPOSITORY>\[-][<SUBPAGE>]

## 选项

- u:打印 URL 而不是打开它.

- C:把 URL 放在剪贴板中,而不是打开它.

- [<USER>/]<REPOSITORY>默认为当前工作目录中的存储库.

- <SUBPAGE>一个"wiki","提交","问题",或其他(默认:"树").

## 例子

```
$ hub browse
> open https://github.com/REPO

$ hub browse -- issues
> open https://github.com/REPO/issues

$ hub browse jingweno/gh
> open https://github.com/jingweno/gh

$ hub browse gh wiki
> open https://github.com/USER/gh/wiki
```

## 更多

hub 比较(1),hub(1)
