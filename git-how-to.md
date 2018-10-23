# GIT COMMANDS

## How to delete branches

git push --delete origin <remotebranchname>
git push origin : <remotebranchname>
git branch -d <localbranchname>
git branch -dr <remote>/<branch>

## how to revert to previous commits

git reset --hard HEAD~1

## how to hide already tracked files

+ git rm -r --cached .
+ git add .
+ git commit -m "message"

## how to re-remote add repository

rm -fr .git
git init
git remote add origin [your-git-remote-url]
git fetch
git reset --mixed origin/master
git branch --set-upstream-to=origin/master master  

## GIT ERRORS

--fatal: unable to access '<remote repo url>': Could not resolve host: github.com
    git config --global --unset http.proxy 
    git config --global --unset https.proxy
    then restart session
