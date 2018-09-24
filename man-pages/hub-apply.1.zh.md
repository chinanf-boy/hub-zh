Hub 应用(1)从 Github 下载补丁并将其应用于本地.= =

## SYNOPSIS

"毂应用"\< Github-URL>

## OPTIONS

- \< Github-URL>:一个在 GUTHUB 上的拉请求或提交的 URL.

## EXAMPLES

```
$ hub apply https://github.com/jingweno/gh/pull/55
>	curl   https://github.com/jingweno/gh/pull/55.patch    ‐o
```

/TMP/55.P 贴

```
> git apply /tmp/55.patch
```

## SEE ALSO

hubAM(1)、hub(1)、GIT 应用(1)
