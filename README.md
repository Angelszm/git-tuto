# Collaborative Repo


## Recommend to use Some GIT GUI Desktop Tool 
- GitHub Desktop (https://desktop.github.com/)
- Sublime Merge (https://www.sublimemerge.com/)
- SourceTree (https://www.sourcetreeapp.com/) 

## Ref : 
- https://www.atlassian.com/git/tutorials/using-branches
- https://gitimmersion.com/lab_01.html

Instructions here :
https://github.com/Angelszm/docker-free-class-for-myanmar

- Git Tutorial
## Session 1
```
- git --version
- git config --global user.name "your_username"
- git config --global user.email "your_emailid"
- git config --list
- git clone https://github.com/Angelszm/git-tuto.git
- git init
- git remote -v ## Track Repo
- git add .
- git commit -m "Message"
- git commit -am "Message"
- git push origin main
- git pull orgin main
- git status 
- git diff (see the changes)
- git checkout -b branch-name
- git branch 
- git branch -r ## remote branch
```


# Lab
- Create new branch with your name 
- Add one file with your name
- Push code


## Session 2: Next Session
### VISUALIZING 
```
- git log (to see very details of every commits)
- git log -2
- git log --oneline
- git log --graph --pretty="%C(yellow) Hash: %h %C(blue)Date: %ad %C(red) Message: %s " --date=human
- git log --graph --pretty="%C(bold blue)%h" --decorate --all
- git log --graph --pretty="%C(yellow) %s"
- git log --graph --pretty='%Cred%h%Creset -%C(auto)%d%Creset %s %Cgreen(%ar) %C(bold blue)<%an>%Creset'
- git log --oneline --abbrev-commit --all --graph --decorate --color
- git log --oneline --abbrev-commit --all --graph
- can use alias 
    - alias gg='git log --oneline --abbrev-commit --all --graph --decorate --color'
    - Ref for alias https://gitimmersion.com/lab_11.html
```

```
- git switch <branch name>
- git fetch (to fetch all of the branches from the repository. )
- git add <file name>
- git stash
- git stash pop 
- git stash apply
- git push --set-upstream origin <branchname> or git push -u origin <branch name>
- git branch --vv (to check upstream branch)
- git reset --hard {Warning!!!}
- git merge <branch name>
- Merging vs Rebasing Option
- get reset --hard with 
- git rebase <branch name>
```


Why Rebase ? 
- Cleaner History
- Linear Project History
- No more unnecessary merge commits
- Don't rebase with other people share projects {SERIOUSLY}

Deleting 
- git checkout master
- git branch -d feature
- git push origin --delete feature
- git branch --all


Cherry Pick to another branch
- git checkout <branch name> 
- git pull origin <branch name> 
- git checkout -b cherry-pick/cp
- git cherry-pick commit-hash-str
- git push -u origin cherry-pick/cp


## Session 3 - Last day of Class
- git revert
- git conflicts 
- git tag 
- git history
- git tag -a <tag-new-version> -m "New Version Updated"
- git push origin <tag-new-version>
- git merge --abort
- git commit -S -m "" https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits


## Example : Merge main branch to another feature branch 
- git checkout main
- git pull
- git checkout -b feature
- git checkout feature
- git merge main
- git commit -m "Merge latest main changes into feature"
- git push origin release/uat

## New Learning: 
```
- git rm --cached (keeps local)
- git rm <file>
- git rm -f <file>
- git rm --cached -r <directory>
- git rm -r <directory>
```


## GitLab Landing Page: 
- Create repo with username/<username>.github.io
- Pages
- Custom Domain


