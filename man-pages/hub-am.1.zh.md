
集线器AM(1)复制从本地GITHUB拉请求提交.= =

## SYNOPSIS

"轮毂AM"[3]\< GITHUB-URL>

## OPTIONS

-   3:(推荐)见GIT-AM(1).

-   \< GITHUB-URL>:一个在GUTHUB上的拉请求或提交的URL.

## EXAMPLES

```
$ hub am ‐3 https://github.com/jingweno/gh/pull/55
>	curl   https://github.com/jingweno/gh/pull/55.patch    ‐o
```

/TMP/55.P贴

```
> git am ‐3 /tmp/55.patch
```

## SEE ALSO

轮毂应用(1),轮毂-樱桃-拾取(1),轮毂(1),GIT -AM(1)
