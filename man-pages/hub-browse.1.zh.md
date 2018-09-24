
Hub浏览(1)在Web浏览器中打开GITHUB存储库.= =

## SYNOPSIS

"集线器浏览"[UC][<USER>/]<REPOSITORY>\[-][<SUBPAGE>]

## OPTIONS

-   u:打印URL而不是打开它.

-   C:把URL放在剪贴板中,而不是打开它.

-   [<USER>/]<REPOSITORY>默认为当前工作目录中的存储库.

-   <SUBPAGE>一个"wiki","提交","问题",或其他(默认:"树").

## EXAMPLES

```
$ hub browse
> open https://github.com/REPO

$ hub browse ‐‐ issues
> open https://github.com/REPO/issues

$ hub browse jingweno/gh
> open https://github.com/jingweno/gh

$ hub browse gh wiki
> open https://github.com/USER/gh/wiki
```

## SEE ALSO

集线器比较(1),集线器(1)
