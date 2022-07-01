# macOS zsh Completions

Some zsh completion files for macOS specific commands and third party tools.

Pull requests and contributions are welcome!

## Setup and Installation

To use mac-zsh-completions on your Mac, follow these steps:

- download the project zip or `git clone` the project
- in your `.zshrc` (or other zsh configuration file) add the full path to the `mac-zsh-completions/completions` directory to the `fpath`, e.g.

```zsh
fpath=( ~/Projects/mac-zsh-completions/completions $fpath )
```

- the command to load `compinit` should come _after_ modifying the `fpath` in your `.zshrc`

- open a new Terminal window to get the new completions

- sometimes (rarely) you may have to delete the `~/.zcompdump` file

```zsh
% rm ~/.zcompdump
% compinit
```

- remember to regularly re-download or `git pull` for new completions and updates

### Install via [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh/)

```zsh
git clone https://github.com/scriptingosx/mac-zsh-completions.git "$ZSH_CUSTOM/plugins/mac-zsh-completions"
```

- Add to your `~/.zshrc` plugins array `plugins=(... mac-zsh-completions)`
- Run `source ~/.zshrc` or restart your shell to activate

## Comments and Discussion

Aside from issues and pull request, I suggest the `#zsh` channel on the [MacAdmins Slack](http://macadmins.org) for discussion.
