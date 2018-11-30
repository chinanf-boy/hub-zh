# hub-delete(1) -- 删除 Github 上的存储库.

## 命令简介

**hub delete** `[-y][<organization>/]<NAME>`

## 选项

- `-y, --yes`:跳过确认提示，并立即删除存储库.

- `[<ORGANIZATION>/]<NAME>`: Github 上存储库的名称.

## 例子

```
$ hub delete recipes
[ personal repo deleted on GitHub ]

$ hub delete sinatra/recipes
[ repo deleted in GitHub organization ]
```

## 更多

[hub-init(1)](hub-init.1.zh.md), [hub(1)](hub.1.zh.md)
