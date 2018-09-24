
Hub创建(1)在Github上创建一个新的存储库,并为它添加一个Git远程.

= =

## SYNOPSIS

"集线器创建"[PoC][‐d <description>] [h<HOMEPAGE>][<有机化>/]<NAME>]

## OPTIONS

-   P:创建一个私有存储库.

-   D<DESCRIPTION>使用此文本作为GITHUB存储库的说明.

-   h<HOMEPAGE>使用此文本作为GITHUB存储库的URL.

-   o,浏览:在Web浏览器中打开新的存储库.

-   c,拷贝:将新存储库的URL放在剪贴板上,而不是打印它.

-   [<ORGANIZATION>/]<NAME>Github上的存储库的名称(默认值:当前工作目录的名称).

    ```
    Optionally, create the repository within <ORGANIZATION>.
    ```

## EXAMPLES

```
$ hub create
[ repo created on GitHub ]
> git remote add ‐f origin git@github.com:USER/REPO.git

$ hub create sinatra/recipes
[ repo created in GitHub organization ]
> git remote add ‐f origin git@github.com:sinatra/recipes.git
```

## SEE ALSO

集线器(1),集线器(1)
