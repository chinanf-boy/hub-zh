hub 远程(1)为 Github 存储库添加 Git 远程.= =

## SYNOPSIS

"hub 远程"添加[P][<options>] <USER>[/<REPOSITORY>]"hub 重置"设置 URL[P][<options>] <NAME> <USER>[/<REPOSITORY>]

## OPTIONS

- P:(弃权)使用远程 URL 的"SSH:"协议.

- <USER>[/<REPOSITORY>]如果<USER>是"原点",那个值将代替你的 Github 用户名.<REPOSITORY>默认为当前工作目录的名称.

## EXAMPLES

```
$ hub remote add jingweno
> git remote add jingweno git://github.com/jingweno/REPO.git

$ hub remote add origin
> git remote add origin git://github.com/USER/REPO.git
```

## SEE ALSO

轮毂叉(1)、轮毂(1)、GIT 遥控器(1)
