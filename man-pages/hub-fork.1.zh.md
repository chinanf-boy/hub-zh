# hub-fork(1) -- 在 Github 上 Fork 当前项目,并为其添加 Git 远程.

## 命令简介

**hub fork** `[--no-remote][--remote-name=<remote>] [--org=<ORGANI-
ZATION>]`

## 选项

- `--no-remote`: Fork 后跳过添加一个 Git 远程.

- `--org=<ORGANIZATION>`: 在这个组织中 Fork 存储库.

## 例子

```
$ hub fork
[ repo forked on GitHub ]
> git remote add -f USER git@github.com:USER/REPO.git

$ hub fork --org=ORGANIZATION
[ repo forked on Github into the ORGANIZATION organization]
>  git  remote  add  -f ORGANIZATION git@github.com:ORGANIZATION/REPO.git
```

## 更多

[hub-clone(1)](hub-clone.1.zh.md), [hub(1)](hub.1.zh.md)
