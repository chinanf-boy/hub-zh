# hub-clone(1) -- 从 GitHub 克隆-clone 库.

## 命令简介

`hub clone` [-p][<options>] [<USER>/]<REPOSITORY> [<DESTINA-
TION>]

## 选项

- -p:(已弃用)克隆 SSH 的私人储存库.

- [<USER>/]<REPOSITORY>: <USER>默认为您自己的 Github 用户名.

- <DESTINATION> 要克隆的目录名(默认:<REPOSITORY>)

## 复制时的协议

"git:"协议将用于克隆公共存储库,而 SSH 协议将用于私有存储库以及,您有访问权限的存储库.另外,hub 可以配置为使用 HTTPS 协议.参见 [hub(1)](hub.1.zh.md) 的 "HTTPS 代替 Git 协议"和"HUB_PROTOCOL".

## 例子

```
$ hub clone rtomayko/ronn
> git clone git://github.com/rtomayko/ronn.git
```

## 更多

[hub-fork(1)](hub-fork.1.zh.md), [hub(1)](hub.1.zh.md), git-clone(1)
