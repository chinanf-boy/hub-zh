# hub-init(1) -- 初始化 Git 存储库,并向 Github 添加远程 remote.

## 命令简介

`hub init` -g

## 选项

- -g:在本地初始化存储库后,添加"origin"远程指向 Github 上的"<USER>/<REPO>"存储库.

```
<USER>  是你的 GitHub 用户名, 而 <REPO>则是当前工作目录的名称.
```

## 例子

```
$ hub init -g
> git init
> git remote add origin git@github.com:USER/REPO.git
```

## 更多

[hub-create(1)](hub-create.1.zh.md), [hub(1)](hub.1.zh.md), git-init(1)
