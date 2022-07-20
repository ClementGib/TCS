# Go Cheat Sheet <img align="center" width="80" height="80" src="https://go.dev/blog/go-brand/Go-Logo/SVG/Go-Logo_Aqua.svg" alt="Go icon">

# Languages
[English](#english-)

## English 🇬🇧🇺🇸

# Contents
1. [Advanced tips](#advanced-tips)
    * [Combined commit](#combined-commit)
    * [Amend](#amend)

### Advanced tips

#### Combined commit

Usually people do `git add` and `git commit` but this is possible do it in one line with `git commit -am`

```bash
# git commit and automatic git add .
$ git commit -am "first commit"
```

You can also create your own command by using `alias`.
This allow you to exec a specific command faster. 
```zsh
# create the ac command  to exec commit -am 
$ git config --global alias.ac "commit -am"
# create the co command to exec checkout
$ git config --global alias.co checkout
# create the br command to exec branch
$ git config --global alias.br branch
# create the ci command to exec commit
$ git config --global alias.ci commit
# create the st command to exec status
$ git config --global alias.st status
```

#### Amend
If you made a mistake during writing your last commit, you can use `amend` to reword it.
```bash
# wrong commit message
$ git commit -am "firsr commit"
# reword last commit
$ git --amend -m "first commit"
```

If you you forgot a files to your last commit you can add it without create an another commit.
```bash
# add forgotten files of current folder
$ git add .
# add files to last commit
$ git --amend --no-edit
```
