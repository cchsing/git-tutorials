# git-tutorials

Tutorials or practices for testing the git features and CLI.<br/>
Following the tutorial on youtube, url: https://www.youtube.com/watch?v=RGOj5yH7evk

## Creating Repo and Cloning the Repo to Local Machine

git clone <url> or
git clone <ssh link>

## Testing the branching of Git

1. Make some modification on the index.html and see how it is reflected in the branch

## Live webpage deployed

URL: https://cchsing.github.io/git-tutorials/

## Method for pushing to Github

1. Create an empty repo on Github
2. Copy the ssh link
3. on the local machine, 'git remote add origin <ssh link>
4. 'git remote -v' to check the config for the remote repo
5. 'git push origin main' or 'git push -u origin main'

## Getting the remote branches

1. `git remote -v` check origin and upstream
2. `git fetch upstream` getting all the branches
3. `git branch -vva` read all the branches
4. `git checkout branch-name` checkout the branch in local repo
5. `git branch -d branch-name` delete branch
6. `git branch -r` see remote branches
7. `git checkout -b fix-failing-tests origin/fix-failing-tests` getting a copy of remote branch
   - it creates a new branch called fix-failing-tests
   - it checkouts that branch
   - it pulls changes from origin/fix-failing-tests to that branch

## Pushing changes

1. touch new-file.js
2. git add .
3. git commit -m "add new file"
4. git push

## merging branch to main

```
$ git checkout master
$ git branch new-branch
$ git checkout new-branch

# ...develop some code...

$ git add –A
$ git commit –m "Some commit message"
$ git checkout master
$ git merge new-branc
```
