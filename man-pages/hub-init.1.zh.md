Hub init(1)初始化 Git 存储库并向 Github 添加远程指向.= =

## 命令简介

"hub 初始化"

## 选项

- g:在本地初始化存储库后,添加"Orthor"远程指向"<USER>/<REPO>"Github 上的知识库".

  ```
  <USER>  is	your GitHub username, while <REPO> is the name of
  ```

  当前工作目录.

## 例子

```
$ hub init -g
> git init
> git remote add origin git@github.com:USER/REPO.git
```

## 更多

毂-创建(1),hub(1),Git -init(1)
