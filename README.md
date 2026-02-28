# terminal-config

# Personal terminal setup (Frappe)
* [Catppuccin Frappe](https://github.com/catppuccin/catppuccin) 
* [Serious Shanns Nerd Font Propo](https://github.com/kaBeech/serious-shanns)
* [Agnoster](https://github.com/agnoster/agnoster-zsh-theme) or [Powerlevel10k](https://github.com/romkatv/powerlevel10k) theme
* Terminal command auto-complete from history: https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md#homebrew
* Git command autocomplete: https://github.com/git/git/blob/master/contrib/completion/git-completion.zsh 
  * In terminal:
```
curl -o ~/.zsh/git-completion.bash https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash
curl -o ~/.zsh/_git https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.zsh
```
  * In .zshrc:
```
fpath=(~/.zsh $fpath)
zstyle ':completion:*:*:git:*' script ~/.zsh/git-completion.bash
autoload -Uz compinit
compinit
```

# Personal terminal setup (Solarized)
* Custom Solarized Dark color scheme: modified from https://github.com/tomislav/osx-terminal.app-colors-solarized
* Meslo LG M Refular for Powerline font: https://github.com/powerline/fonts
* Agnoster theme: https://github.com/agnoster/agnoster-zsh-theme

## Setup
1. Install Antigen: https://github.com/zsh-users/antigen
2. Install Powerline fonts: https://github.com/powerline/fonts
3. Pull files from this repo into root level directory
4. Restart terminal and enjoy!

## Troubleshooting
### Ignore insecure directories and continue [y] or abort compinit [n]
Run `compaudit` to see list of insecure directories
Run `sudo chmod -R 755 {path}` to change permissions on directories

# Personal VSCode setup
* Rouge color scheme
* Customized IDE behavior and keybindings
* Plugins
  * Docker
  * ESLint
  * GitLens — Git supercharged
  * Jest
  * Jira and BitBucket (Official)
  * Markdown All in One
  * Remote - Containers
  * vscode-proto3
  * yaml
  * Rouge Theme

## Setup
1. Navigate to `~/Library/Application Support/Code/User` and paste the files inside this repo's VSCode directory there
