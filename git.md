# Go Cheat Sheet <img align="center" width="80" height="80" src="https://go.dev/blog/go-brand/Go-Logo/SVG/Go-Logo_Aqua.svg" alt="Go icon">

# Languages
[English](#english-)

## English 🇬🇧🇺🇸

# Contents
1. [Advanced tips](#advanced-tips)

### Advanced tips

#### Combined commit

Usually people do `git add` and `git commit` but this is possible do it in one line with `git commit -am`

```bash
# automatic git add .
$ git commit -am "first commit"
```

You can also create your own command by using `alias`.
This allow you to exec a specific command faster. 
```bash
# create command ac to exec commit -am 
$ git config --global alias.ac "commit -am"
# create command co to exec checkout
$ git config --global alias.co checkout
# create command br to exec branch
$ git config --global alias.br branch
# create command ci to exec commit
$ git config --global alias.ci commit
# create command st to exec status
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
