
Hub init(1)初始化Git存储库并向GITHUB添加远程指向.= =

## SYNOPSIS

"集线器初始化"

## OPTIONS

-   g:在本地初始化存储库后,添加"Orthor"远程指向"<USER>/<REPO>"Github上的知识库".

    ```
    <USER>  is	your GitHub username, while <REPO> is the name of
    ```

    当前工作目录.

## EXAMPLES

```
$ hub init ‐g
> git init
> git remote add origin git@github.com:USER/REPO.git
```

## SEE ALSO

毂-创建(1),集线器(1),Git -init(1)
