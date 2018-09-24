hub 获取(1)在执行 Git 之前添加丢失的远程文件

# fetch.

## 命令简介

"hub 读取"<USER>[,<USER2>...…]

## 例子

```
$ hub fetch --multiple jingweno mislav
> git remote add jingweno git://github.com/jingweno/REPO.git
> git remote add mislav git://github.com/mislav/REPO.git
> git fetch jingweno
> git fetch mislav
```

## 更多

hub-远程(1),hub(1),Git -FETCH(1)
