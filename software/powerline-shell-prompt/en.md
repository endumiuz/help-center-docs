+++
title = "Powerline Shell Prompt"
lastmod = "2020-02-05T22:20:41+01:00"
+++
# Powerline Shell Prompt

[Powerline](https://github.com/powerline) is a statusline plugin for vim, and provides statuslines and prompts for several other applications, including zsh, bash, tmux, IPython, Awesome and Qtile.

## Installation

Powerline has two components, the plugin system itself ([powerline](https://dev.getsol.us/source/powerline/)) and the fonts ([powerline-fonts](https://dev.getsol.us/source/powerline-fonts/)). Both are available in the Software Center or via eopkg in a terminal:

``` bash
sudo eopkg it powerline powerline-fonts
```

## Shell Prompts

To get Powerline working inside your terminal, you need to add some commands to your shell configuration file.

### Bash

Add the following commands to `~/.bashrc`

``` bash
powerline-daemon -q
POWERLINE_BASH_CONTINUATION=1
POWERLINE_BASH_SELECT=1
source /usr/lib/python3.7/site-packages/powerline/bindings/bash/powerline.sh
```

### Busybox and dash

Add the following commands to `[INSERT CONFIG FILE]`

``` bash
powerline-daemon -q
source /usr/lib/python3.7/site-packages/powerline/bindings/shell/powerline.sh
powerline-setup
```

### Fish

Add the following commands to `~/.config/fish/config.fish`.

``` bash
powerline-daemon -q
source /usr/lib/python3.7/site-packages/powerline/bindings/fish/powerline-setup.fish
powerline-setup
```

### Zsh

Add the following commands to `~/.zshrc`.

``` bash
powerline-daemon -q
source /usr/lib/python3.7/site-packages/powerline/bindings/zsh/powerline.zsh
powerline-setup
```

Read more about Powerline inside the Docs [Link](https://powerline.readthedocs.io/en/master/usage/shell-prompts.html#)
