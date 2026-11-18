# Using Git & Github

## SSH to Github
1. Generate ssh key `ssh-keygen -t ed25519 -C "email@example.com"`
2. Copy .pub to github.com > profile picture > Settings > SSH and GPG Keys > New SSH Key

## Global Git options to change
- `git config --global user.name`
- `git config --global email`
- `export EDITOR=vi` - Change default editor from nano to vi

## Common commands
- `git init` - create git repo in current directory
- `git add` - move file(s) to staging area. add multiple files using `git add .`
- `git commit -m "comment"` - takes staging area items and records them as a snapshot in local repo. Basically saving your work 
- `git remote add origin git@github.com:USERNAME/myproject.git` - told git where Github is. 
- `git push -u origin master` - push changes to git
- `git diff` - show changes from master and current
- `git status` - show what stage your changes are in
- `git log` - show commit history

Common workflow is edit file > `git add` > `git commit` > `git push`

## Create a branch
`git switch -c branch-name` - This will create a branch and switches you to it. You can confirm with `git branch`
- From here you can perform edits on your branch then add, commit, and push. The first `git push` will require the `-u` parameter, refer to error message
- Delete old branches with `git branch -d branch-name`

### Pull Requests (PR)
Pull requests allow for code review, discussion, QA and history view. Viewing PRs can be done through CLI but just use GitHub for now. When you're done reviewing the code and want to merge it, you can click *Merge pull request* > *Confirm Merge* > *Delete branch* (to keep things clean)

#### Update Local repo
`git switch master` - you'll notice that git will tell you if your master branch is behind. Use `git pull` to update

## Clone repositories
To work on existing open source projects you can use `git clone`. This is a tiny public practice repo
```
git clone https://github.com/octocat/Hello-World.git
```


