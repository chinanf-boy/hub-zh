
hub签出(1)-检查拉请求的头作为LO分支.= =

## SYNOPSIS

"hub签出"\< PulrReq URL >[<BRANCH>]

## EXAMPLES

```
$ hub checkout https://github.com/jingweno/gh/pull/73
> git fetch origin pull/73/head:jingweno‐feature
> git checkout jingweno‐feature
```

## SEE ALSO

hub合并(1)、hubAM(1)、hub(1)、GIT校验(1)
