# hub-remote(1) -- 为 Github 存储库添加 Git 远程-remote.

## 命令简介

`hub remote` add [-p][<options>] <USER>[/<REPOSITORY>] `hub re- mote` set-url [-p][<options>] <NAME> <USER>[/<REPOSITORY>]

## 选项

- -p:(已弃用)) 使用"SSH:"协议.远程 URL

- <USER>[/<REPOSITORY>] 如果<USER>是"origin",那个值将是你的 Github 用户名.<REPOSITORY>默认为当前工作目录的名称.

## 例子

```
$ hub remote add jingweno
> git remote add jingweno git://github.com/jingweno/REPO.git

$ hub remote add origin
> git remote add origin git://github.com/USER/REPO.git
```

## 更多

[hub-fork(1)](hub-fork.1.zh.md), [hub(1)](hub.1.zh.md), git-remote(1)
