# hub-create(1) -- 在 Github 上创建一个新的存储库,并为其添加 Git 远程.

## 命令简介

`hub create` [-poc][-d <description>] [-h <HOMEPAGE>][<ORGANI-
ZATION>/]<NAME>]

## 选项

- -p :创建一个私有存储库.

- -d <DESCRIPTION>: 使用此文本作为 Github 存储库的说明.

- -h <HOMEPAGE>: 使用此文本作为 Github 存储库的 URL.

- -o, --browse:在 Web 浏览器中打开新的存储库.

- -c ,拷贝:将新存储库的 URL 放在剪贴板上,而不是打印它.

- [<ORGANIZATION>/]<NAME>: Github 上的存储库的名称(默认值:当前工作目录的名称).

```
很显然, 在<ORGANIZATION>下创建存储库.
```

## 例子

```
$ hub create
[ repo created on GitHub ]
> git remote add -f origin git@github.com:USER/REPO.git

$ hub create sinatra/recipes
[ repo created in GitHub organization ]
> git remote add -f origin git@github.com:sinatra/recipes.git
```

## 更多

[hub-init(1)](hub-init.1.zh.md), [hub(1)](hub.1.zh.md)
