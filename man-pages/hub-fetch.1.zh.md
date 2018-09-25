# hub-fetch(1) -- 在执行 Git 获取之前,添加错过的 remote

## 命令简介

`hub fetch` <USER>[,<USER2>...]

## 例子

```
$ hub fetch --multiple jingweno mislav
> git remote add jingweno git://github.com/jingweno/REPO.git
> git remote add mislav git://github.com/mislav/REPO.git
> git fetch jingweno
> git fetch mislav
```

## 更多

[hub-remote(1)](hub-remote.1.zh.md), [hub(1)](hub.1.zh.md), git-fetch(1)
