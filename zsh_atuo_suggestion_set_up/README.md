# Iterm2 with command auto suggestion.

![image](https://github.com/function-hub/Utilities/blob/master/images/autosuggest.gif)

## Install iterm2 and oh-my-zsh (macOS)

link: https://www.iterm2.com/

## Enabling Plugins (zsh-autosuggestions & zsh-syntax-highlighting)

- Download zsh-autosuggestions by

`git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions`

- `cat ~/.zshrc` find `plugins=(git)`

- Append `zsh-autosuggestions & zsh-syntax-highlighting` to `plugins()` like this

`plugins=(git zsh-autosuggestions zsh-syntax-highlighting)`

- Reopen iterm2

### Ref

- [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
- [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)
- [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)
