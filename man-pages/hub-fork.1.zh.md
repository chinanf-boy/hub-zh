Hub 分支(1)将当前项目在 Github 上添加,并为其添加 Git 远程.

## 命令简介

毂叉[远程遥控器][--remote-name=<remote>] [Org=<有机化>]

## 选项

- 非远程:跳过为叉添加一个 Git 远程.

- Orgorg=<ORGANIZATION>在这个组织中拨存储库.

## 例子

```
$ hub fork
[ repo forked on GitHub ]
> git remote add -f USER git@github.com:USER/REPO.git

$ hub fork --org=ORGANIZATION
[ repo forked on Github into the ORGANIZATION organization]
>  git  remote  add  -f ORGANIZATION git@github.com:ORGANIZA-
```

GIT

## 更多

hub 克隆(1),hub(1)
