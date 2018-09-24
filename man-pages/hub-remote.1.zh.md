
集线器远程(1)为GITHUB存储库添加Git远程.= =

## SYNOPSIS

"集线器远程"添加[P][<options>] <USER>[/<REPOSITORY>]"集线器重置"设置URL[P][<options>] <NAME> <USER>[/<REPOSITORY>]

## OPTIONS

-   P:(弃权)使用远程URL的"SSH:"协议.

-   <USER>[/<REPOSITORY>]如果<USER>是"原点",那个值将代替你的Github用户名.<REPOSITORY>默认为当前工作目录的名称.

## EXAMPLES

```
$ hub remote add jingweno
> git remote add jingweno git://github.com/jingweno/REPO.git

$ hub remote add origin
> git remote add origin git://github.com/USER/REPO.git
```

## SEE ALSO

轮毂叉(1)、轮毂(1)、GIT遥控器(1)
