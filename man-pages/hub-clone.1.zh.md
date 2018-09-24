Hub 克隆(1)从 Github 中克隆一个存储库.= =

## SYNOPSIS

"中枢克隆"[P][<options>] [<USER>/]<REPOSITORY> [<命运> ]

## OPTIONS

- P:(弃权)克隆 SSH 的私人储存库.

- [<USER>/]<REPOSITORY>:<USER>默认为您自己的 Github 用户名.

- <DESTINATION>要克隆的目录名(默认:<REPOSITORY>)

## PROTOCOL USED FOR CLONING

"git:"协议将用于克隆公共存储库,而 SSH 协议将用于私有存储库以及您有强制访问权限的存储库.另外,hub 可以配置为使用 HTTPS 协议.参见"HTTPS 代替 Git 协议"和"Hubl 协议"的 hub(1).

## EXAMPLES

```
$ hub clone rtomayko/ronn
> git clone git://github.com/rtomayko/ronn.git
```

## SEE ALSO

轮毂叉(1)、轮毂(1)、GIT -克隆(1)
