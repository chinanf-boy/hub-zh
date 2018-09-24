Hub 创建(1)在 Github 上创建一个新的存储库,并为它添加一个 Git 远程.

= =

## 命令简介

"hub 创建"[PoC][-d <description>] [h<HOMEPAGE>][<有机化>/]<NAME>]

## 选项

- P:创建一个私有存储库.

- D<DESCRIPTION>使用此文本作为 Github 存储库的说明.

- h<HOMEPAGE>使用此文本作为 Github 存储库的 URL.

- o,浏览:在 Web 浏览器中打开新的存储库.

- c,拷贝:将新存储库的 URL 放在剪贴板上,而不是打印它.

- [<ORGANIZATION>/]<NAME>Github 上的存储库的名称(默认值:当前工作目录的名称).

  ```
  Optionally, create the repository within <ORGANIZATION>.
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

hub(1),hub(1)
