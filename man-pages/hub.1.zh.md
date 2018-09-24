# hub(1) - 让 git 与 github 更容易合作

## 命令简介

- "hub" [`-noop`] <COMMAND> [<OPTIONS>]
- "hub alias" [`-s`][<shell>]
- "hub-help" - <COMMAND>

## DESCRIPTION

hub 是一个 Git 包装工具 ,为了扩展与额外的功能,让它更好的在 GitHub 工作.

## 命令

可分为两组: al- 所有这些都是在 Git 现成的, hub 扩展了和 hub 提供的是 cus-.

### 扩展的 git 命令

- [hub-am(1)](./hub-am.1.zh.md):从 Github 的(pull request)提交请求复制 commit 到本地.

- [hub-apply(1)](./hub-apply.1.zh.md): 从 GitHub 下载补丁和本地应用.

- [hub-checkout(1)](./hub-checkout.1.zh.md): 签到-Checkout 提交请求的 head 作为一个本地分支.

- [hub-cherry-pick(1)](./hub-cherry-pick.1.zh.md): 从 Github 的一个 Fork 选择一个 commit.

- [hub-clone(1)](./hub-clone.1.zh.md):从 GitHub 克隆-clone 库.

- [hub-fetch(1)](./hub-fetch.1.zh.md):在执行 Git 获取之前,添加丢失的 remote.

- [hub-init(1)](./hub-init.1.zh.md):初始化 Git 存储库,并向 Github 添加远程 remote.

- [hub-merge(1)](./hub-merge.1.zh.md):将 一个本地带信息的提交请求合并,就像在 Github 的 Merge 按钮.

- [hub-push(1)](./hub-push.1.zh.md):将 Git 分支推到每个远程-remote 列表上.

- [hub-remote(1)](./hub-remote.1.zh.md):为 Github 存储库添加 Git 远程-remote.

- [hub-submodule(1)](./hub-submodule.1.zh.md):为 Github 存储库添加 Git 子模块.

### hub 提供的新命令

- [hub-alias(1)](./hub-alias.1.zh.md):显示用于包装 Git 的 shell 指令.

- [hub-browse(1)](./hub-browse.1.zh.md):在 Web 浏览器中打开 Github 存储库.

- [hub-ci-status(1)](./hub-ci-status.1.zh.md):显示提交-commit 的 Github 状态信息.

- [hub-compare(1)](./hub-compare.1.zh.md):在 Web 浏览器中打开 Github 比较页.

- [hub-create(1)](./hub-create.1.zh.md):在 Github 上创建一个新的存储库,并为其添加 Git 远程.

- [hub-delete(1)](./hub-delete.1.zh.md):删除 Github 上的存储库.

- [hub-fork(1)](./hub-fork.1.zh.md):在 Github 上 Fork 当前项目,并为其添加 Git 远程.

- [hub-pull-request(1)](./hub-pull-request.1.zh.md):创建 Github 拉请求.

- [hub-pr(1)](./hub-pr.1.zh.md):列出和签到-checkout Github 提交请求.

- [hub-issue(1)](./hub-issue.1.zh.md):列出和创建 Github 问题.

- [hub-release(1)](./hub-release.1.zh.md):列出,并创建 Github 版本.

- [hub-sync(1)](./hub-sync.1.zh.md):从上游获取,并更新本地分支.

## 配置

### GitHub OAuth 安全验证

Hub 在第一次需要访问 API 时,将按照提示输入 GitHub 用户名和密码,并将其交换为 OAuth 令牌,并将其保存在`~/.config/hub`中.

为了避免被提示,使用"GITHUB_USER"和"GITHUB_PASSWORD"环境变量.

或者,您可以提供"GITHUB_TOKEN",一个访问令牌.**存储库**权限.这将不会写到"~/.con-
fig/hub".

### 用 HTTPS 替换 git 协议

如果您更喜欢 HTTPS 协议用于 git 操作,那么您可以通过配置 hub 来生成"https\:"-URLs,而不是"git:"或"ssh:":

```
$ git config -global hub.protocol https
```

这将影响"clone"、"fork"、"remote add"和其他对 GitHub 库的 URL 引用的 hub 扩展命令.

### GitHub Enterprise-企业

默认情况下,hub 只与具有指向"github.com"的存储库一起工作.Github 企业主机需要用白名单配置 hub ,处理与 github.com 相同的远程服务器:

```
$ git config -global -add hub.host MY.GIT.ORG
```

诸如"init"和"clone"等命令的默认主机仍然是"github.com",但这可受到"GITHUB_HOST"环境变量的影响:

```
$ GITHUB_HOST=my.git.org git clone myproject
```

### 环境变量

- "HUB_VERBOSE": hub 命令启用 verbose 的输出.

- "HUB_CONFIG":读取和存储 hub 配置的文件路径.如果存在"XDG_CONFIG_HOME",则默认值为"$XDG_CONFIG_HOME/hub"; 否则为"$HOME/.config/hub".每个 XDG 基础目录规范,也可在"XDG_CONFIG_DIRS"中搜索配置文件.

- "‘HUB_PROTOCOL‘":使用其中一个"https|ssh|git" 作为 git clone/push 的首选协议.

- ‘GITHUB_TOKEN‘:用于 Github API 请求的 OAuth 令牌.

## BUGS

[HTTPS://GithubCOM/github/Hub/问题](https://github.com/github/hub/issues)

## 作者

[HTTPS://GithubCOM/Github/HUB/贡献者](https://github.com/github/hub/contributors)

## 更多

git(1), git-clone(1), git-remote(1), git-init(1),
https://github.com/github/hub
