
集线器签出(1)-检查拉请求的头作为LO分支.= =

## SYNOPSIS

"集线器签出"\< PulrReq URL >[<BRANCH>]

## EXAMPLES

```
$ hub checkout https://github.com/jingweno/gh/pull/73
> git fetch origin pull/73/head:jingweno‐feature
> git checkout jingweno‐feature
```

## SEE ALSO

集线器合并(1)、集线器AM(1)、集线器(1)、GIT校验(1)
