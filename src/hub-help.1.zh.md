# hub-help(1) -- 显示命令的帮助页

## 命令简介

- **hub help** `hub `
- **hub help** `<COMMAND> `
- **hub help** `hub-<COMMAND>
 [--plain-text]`

## 选项

- `hub-<COMMAND>`:
  使用此格式查看对存在的 Git 命令的 hub 扩展的帮助.

- `--plain-text`:
  跳过 man 页查找机制并,显示普通帮助文本.

## MAN 查看机制

在具有"man"的系统中,帮助页面安装相对于"hub"前缀,可在这些双字串中查找:

- ‘man/<command>.1‘
- ‘share/man/man1/<command>.1‘

在没有"man"的系统中,相同的帮助页用".txt"后缀查找.

## 更多

hub(1), git-help(1)
