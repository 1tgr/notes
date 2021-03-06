# Aliases
```bash
vim ~/.gitconfig
```

Add to the bottom:
```
[alias]
lg1 = log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all
lg2 = log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold cyan)%aD%C(reset) %C(bold green)(%ar)%C(reset)%C(bold yellow)%d%C(reset)%n''          %C(white)%s%C(reset) %C(dim white)- %an%C(reset)' --all
lg = !"git lg1"
```
(from https://stackoverflow.com/a/9074343)

# `git pull` rebases instead of merges
```bash
git config --global --bool pull.rebase true
```

# Automatically `prune` local copy of remote branches when they're deleted from the remote
```bash
git config --global --bool fetch.prune true
```
