# ubuntu-termianl-settings
my custom zsh settings and other bash settings.

## Install zsh: 

```
sudo apt install git-core zsh
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
sudo apt install fonts-powerline

<!-- Open up ~/.zshrc and change ZSH_THEME variable: -->
ZSH_THEME="agnoster"
```

## Customize terminal
* Go to home: `cd ~`
* Add following settings at the end of `.zshrc` file
<!-- source: https://github.com/robbyrussell/oh-my-zsh/issues/5479 -->
```
prompt_dir () {
    prompt_segment blue black "${PWD##*/}"
}
export DEFAULT_USER="$(whoami)" # remove username@laptop info from terminal
```

## Sample .zshrc available in repo
