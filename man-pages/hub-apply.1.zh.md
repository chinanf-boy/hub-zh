
Hub应用(1)从GITHUB下载补丁并将其应用于本地.= =

## SYNOPSIS

"毂应用"\< GITHUB-URL>

## OPTIONS

-   \< GITHUB-URL>:一个在GUTHUB上的拉请求或提交的URL.

## EXAMPLES

```
$ hub apply https://github.com/jingweno/gh/pull/55
>	curl   https://github.com/jingweno/gh/pull/55.patch    ‐o
```

/TMP/55.P贴

```
> git apply /tmp/55.patch
```

## SEE ALSO

集线器AM(1)、集线器(1)、GIT应用(1)
