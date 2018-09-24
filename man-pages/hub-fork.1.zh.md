
Hub分支(1)将当前项目在GITHUB上添加,并为其添加Git远程.

## SYNOPSIS

毂叉[远程遥控器][‐‐remote‐name=<remote>] [Org=<有机化>]

## OPTIONS

-   非远程:跳过为叉添加一个Git远程.

-   Orgorg=<ORGANIZATION>在这个组织中拨存储库.

## EXAMPLES

```
$ hub fork
[ repo forked on GitHub ]
> git remote add ‐f USER git@github.com:USER/REPO.git

$ hub fork ‐‐org=ORGANIZATION
[ repo forked on Github into the ORGANIZATION organization]
>  git  remote  add  ‐f ORGANIZATION git@github.com:ORGANIZA‐
```

GIT

## SEE ALSO

集线器克隆(1),集线器(1)
