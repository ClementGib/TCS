# Git Cheat Sheet <img align="center" width="80" height="80" src="https://upload.wikimedia.org/wikipedia/commons/e/e0/Git-logo.svg" alt="Go icon">

# Languages
[English](#english-)

## English 🇬🇧 🇺🇸

# Contents
1. [Advanced tips](#advanced-tips)
    * [Combined commit](#combined-commit)
    * [Amend](#amend)

### Advanced tips

#### Combined commit ⏩

Usually people do `git add` and `git commit` but this is possible do it in one line with `git commit -am "message"`. <br>
This command followed by the commit message will automaticly add files of the current folder and commit with a message
```bash
# git commit and automatic git add .
$ git commit -am "first commit"
```

You can also create your own command by using `alias`.✨ <br>
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

#### Amend 📝
If you made a mistake during writing your last commit, you can use `amend` to reword it.
```bash
# wrong commit message
$ git commit -am "first commiir"
# reword last commit
$ git commit --amend -m "first commit"
```

If you forgot files into your last commit, you can add it without create an another commit.
```bash
# add forgotten files of current folder
$ git add .
# add files to last commit
$ git commit --amend --no-edit
```


#### Push ➡️
⛔ If you do an ordinary push it can be rejected for many reason:
- You rebased your branch onto master
- You reordered the commits
- You changed the commit messages
- You squashed the commits into one

In this case you can use `--force` or the short version `-f`, to bypass all the restriction right ?
If someone pushed a new commit before you and you don't have the last version of the branch, you will erase his commit forever... 💀

To avoid that, one can instead use the `git push --force-with-lease` command.git gonna check if the remote version of the branch is the same as the one you rebase and if someone push new commits when we were rebasing. The push is then rejected if the remotes branch is changed! ⛔
```bash
# push if base branch is the same
git push --force-with-lease
```

#### Revert 
...