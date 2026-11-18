# Common commands
`git init` - create git repo in current directory
`git add` - move file(s) to staging area. add multiple files using `git add .`
`git commit -m "comment"` - takes staging area items and records them as a snapshot in local repo. Basically saving your work 
`git remote add origin git@github.com:USERNAME/myproject.git` - 
`git push -u origin master` - push changes to git
`git diff` - show changes from master and current
`git status`
`git log`

Common workflow is edit file > `git add` > `git commit` > `git push`

## Global Git options to change
git config --global user.name
git config --global email
- Change default editor from nano to vi
export EDITOR=vi


# Use SSH for Git
1. Generate ssh key `ssh-keygen -t ed25519 -C "email@example.com"`
2. Copy .pub to github.com > profile picture > Settings > SSH and GPG Keys > New SSH Key
