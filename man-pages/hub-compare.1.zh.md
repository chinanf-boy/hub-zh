
# hub‐compare(1)	‐‐  Open  a GitHub compare page in a web browser.

## SYNOPSIS

"集线器比较"[U][‐b <base>] [<USER>][<START>...…]<END>]

## OPTIONS

-   u:打印URL而不是打开它.

-   C,拷贝:把URL放在剪贴板上,而不是打开它.

-   乙<BASE>基础分支进行比较.

-   [<START>...…]<END>指定要比较的范围的分支名称、标签名或提交SAS.<END>默认为当前分支名称.

    ```
    If a range with two dots (‘A..B‘) is given, it will be trans‐
    ```

    形成一个有三个点的范围.

## EXAMPLES

```
$ hub compare refactor
> open https://github.com/USER/REPO/compare/refactor

$ hub compare v1.0..v1.1
> open https://github.com/USER/REPO/compare/v1.0...v1.1

$ hub compare ‐u jingweno feature
> echo https://github.com/jingweno/REPO/compare/feature
```

## SEE ALSO

集线器浏览(1),集线器(1)
