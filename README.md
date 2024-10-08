<!-- Git Tutorial-->

# In this tutorial we will learn all the git commands

---
<p>1. First of all initialize the git in the work directory.</p>

```
git init
```

<p>2. For showing all the files or folder from working directory.</p>

```
i.  git ls
ii. git ls -a
```

<p>3. Git uses three-tri architecture such as:</p>

```
1. working directory
2. staging area
3. local repository

working directory ---> staging area  --->  local repository
```

<p>4. The command is use for identify the git architechter.</p>

```
git status
```
<p>5. For showing the changes into the working directory.</p>

```
git diff
```
<p>6. How can understand which layer we are staying?</p>

`red color for working directory` </br>

`blue color for staging area`
<p>7. To move working directory to staging area:<p/>

```
There are different ways

// for specific files -- with extension
1. git add filename1 filename2 ...

// for all the file which are the same extension
2. git add *.extension

// all the file of the directory -- alson different extension fils
3. git add .
```
<p>8. To move back the staging area to working directory.</p>

```
git restore filename
```
<p>9. To move the staging area to local repository:</p>

```
git commit -m "clean message for changes"
```
<p>10. For showing all the commits you have done.</p>

```
// with full commitID
1. git log

//short commitID
2. git log --oneline
```
<p>11. For showing the changes after commit:</p>

```
1. git show
2. git show head
```
<p>12. Move one branch to another branch:</p>

```
git checkout commit_id

```
Always remember, the letest commit id always `master`
<p>13. For go back to the previous layer:</p>

```
// local repository to staging area
1. git reset --soft HEAD^

// local repository to working directory -- with recent changes
2. git reset HEAD^

// local repo to working directory -- with delete recent changes
3. git reset --hard HEAD
```
<p>14. git revert is most important for the developer. git reset removed the commit history, but revert does not do that:</p>

`git revert commit_id`


<p>15. For upload the code from local repository to remote repository</p>

```
step-1: first complete adding and commiting into the local repo

step-2: connect with the remote repo.
--> git remote add origin 'github_repo_link'

step-3: git branch -M main

step-4: git push -u origin main
```

<p>16. pull command work for taking codes from remote repo to local repo.</p>

`git pull origin branch_name`
if you stay in the same branch then just use `git pull`

<p>17. For checking the local repo is connected or not with remote repo.</p>

`git remote -v`

18. show branch `git branch`

19. create branch
```
git branch new_branch_name
```
20. move different branch `git checkout branchName`

- Here we create a branch name develop and make a commit but If we move the main branch then we didnot find the file which created in the develop branch.

Please complete adding and commiting all the from new branch then move to the main branch.

### Merge two branch
1. Merge data from develop branch to main branch. Ensure done commit in the develop branch.

2. Back to the main branch and press `git merge develop`

3. Data will be added into the main branch. After delete the develop branch. `git branch -d develop`

## push code to the specific branch
1. If you staying `develop` branch and you want to push data to the `develop` branch the just write `git push`

2. If you staying `develop` branch and you want to push to the `main` branch then the command is `git push -u origin main`