
# 安装说明

## bash+Homebrew

如果你使用Homebrew软件,只需运行`brew install hub`应该自动完成了.

## bash

在Linux上打开你的`.bashrc`文件,或者在MaOS上`.bash_profile`,添加:

```sh
if [ -f /path/to/hub.bash_completion ]; then
  . /path/to/hub.bash_completion
fi
```

## zsh

从你下载`hub`的文件夹位置,复制`etc/hub.zsh_completion`文件到`~/.zsh/completions/`并将其重命名为`_hub`:

```sh
mkdir -p ~/.zsh/completions
cp etc/hub.zsh_completion ~/.zsh/completions/_hub
```

然后将下列行添加到您的`.zshrc`文件:

```sh
fpath=(~/.zsh/completions $fpath) 
autoload -U compinit && compinit
```

## fish

从你下载`hub`的文件夹位置,复制`etc/hub.fish_completion`文件到`~/.config/fish/completions/`并将其重命名为`hub.fish`:

```sh
mkdir -p ~/.config/fish/completions
cp etc/hub.fish_completion ~/.config/fish/completions/hub.fish
```
