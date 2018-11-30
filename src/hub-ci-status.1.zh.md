# hub-ci-status(1) -- 显示提交-commit 的 Github 状态信息.

## 命令简介

**hub ci-status** `[-v][\<COMMIT\>]`

## 选项

- `-v`:打印所有状态检查和 URL 的详细报告.

- `<COMMIT>`: 一个提交或分支名称(默认:"HEAD").

可能的输出和退出状态:

- 成功,默认:0
- 失败,错误,行动需要,超时:1
- 等待:2

## 更多

[hub-pull-request(1)](hub-pull-request.1.zh.md), [hub(1)](hub.1.zh.md)
