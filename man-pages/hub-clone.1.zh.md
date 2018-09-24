
Hub克隆(1)从Github中克隆一个存储库.= =

## SYNOPSIS

"中枢克隆"[P][<options>]  [<USER>/]<REPOSITORY> [<命运> ]

## OPTIONS

-   P:(弃权)克隆SSH的私人储存库.

-   [<USER>/]<REPOSITORY>:<USER>默认为您自己的GITHUB用户名.

-   <DESTINATION>要克隆的目录名(默认:<REPOSITORY>)

## PROTOCOL USED FOR CLONING

"git:"协议将用于克隆公共存储库,而SSH协议将用于私有存储库以及您有强制访问权限的存储库.另外,集线器可以配置为使用HTTPS协议.参见"HTTPS代替Git协议"和"Hubl协议"的集线器(1).

## EXAMPLES

```
$ hub clone rtomayko/ronn
> git clone git://github.com/rtomayko/ronn.git
```

## SEE ALSO

轮毂叉(1)、轮毂(1)、GIT -克隆(1)
