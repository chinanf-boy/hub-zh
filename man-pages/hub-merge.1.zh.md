
Hub合并(1)将拉取请求与GITHUB合并按钮类似地合并在一起.= =

## SYNOPSIS

"集线器合并"\< PulrReq URL >

这在当前分支中创建了本地合并提交,但实际上没有改变拉取请求的状态.但是,当新创建的合并提交被推送到远程存储库的默认分支时,拉请求将自动关闭并标记为"合并".

## EXAMPLES

```
$ hub merge https://github.com/jingweno/gh/pull/73
> git fetch origin refs/pull/73/head
> git merge FETCH_HEAD ‐‐no‐ff ‐m  "Merge  pull  request  #73
```

来自京文/特写…

## SEE ALSO

集线器校验(1)、集线器(1)、Git合并(1)