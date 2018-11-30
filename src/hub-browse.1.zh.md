# hub-browse(1) -- 在 Web 浏览器中打开 Github 存储库.

## 命令简介

**hub browse** `[-uc][<USER>/]<REPOSITORY>|--] [<SUBPAGE>]`

## 选项

- `-u`: 打印 URL ,而不是打开它.

- `-c`: 把 URL 放在剪贴板中,而不是打开它.

- `[<USER>/]<REPOSITORY>`:默认为当前工作目录中的存储库.

- `<SUBPAGE>`:"wiki","commits","issues"其中一个,或其他(默认:"tree").

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

[hub-compare(1)](hub-compare.1.zh.md), [hub(1)](hub.1.zh.md)
