hubAM(1)复制从本地 Github 拉请求提交.= =

## SYNOPSIS

"轮毂 AM"[3]\< Github-URL>

## OPTIONS

- 3:(推荐)见 GIT-AM(1).

- \< Github-URL>:一个在 GUTHUB 上的拉请求或提交的 URL.

## EXAMPLES

```
$ hub am ‐3 https://github.com/jingweno/gh/pull/55
>	curl   https://github.com/jingweno/gh/pull/55.patch    ‐o
```

/TMP/55.P 贴

```
> git am ‐3 /tmp/55.patch
```

## SEE ALSO

轮毂应用(1),轮毂-樱桃-拾取(1),轮毂(1),GIT -AM(1)
