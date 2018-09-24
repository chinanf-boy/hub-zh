# hub-compare(1) -- Open a GitHub compare page in a web browser.

## 命令简介

"hub 比较"[U][-b <base>] [<USER>][<start>...…]<END>]

## 选项

- u:打印 URL 而不是打开它.

- C,拷贝:把 URL 放在剪贴板上,而不是打开它.

- 乙<BASE>基础分支进行比较.

- [<START>...…]<END>指定要比较的范围的分支名称、标签名或提交 SAS.<END>默认为当前分支名称.

  ```
  If a range with two dots (`A..B`) is given, it will be trans-
  ```

  形成一个有三个点的范围.

## 例子

```
$ hub compare refactor
> open https://github.com/USER/REPO/compare/refactor

$ hub compare v1.0..v1.1
> open https://github.com/USER/REPO/compare/v1.0...v1.1

$ hub compare -u jingweno feature
> echo https://github.com/jingweno/REPO/compare/feature
```

## 更多

hub 浏览(1),hub(1)
