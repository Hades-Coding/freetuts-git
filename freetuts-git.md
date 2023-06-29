# With GITHUB - default is main, not master, so sould rename it to master
# git branch --move main master
# git push --set-upstream [remote_repo_name] master
# Change default remote repository: https://github.com/settings/repositories
# Authen Key: https://github.com/settings/keys

# Config first
git config --global init.defaultBranch master
git config --global user.name Hades
git config --global user.email o352180877@gmail.com
git status

# Initial first, then save credential
git init
git config credential.helper store

# Add 1st file to local repo
git add freetuts-git.md
git commit -m "1st file on branch master"

# Only map remote when you have local repo
# git remote

git remote -v 
git remote add git-remote https://github.com/Hades-Coding/freetuts-git.git
git remote -v

# create remote repository on GITHUB first, eg: freetuts-git

# update local to remote repository
# git push --set-upstream git-remote master
git push -u git-remote master
