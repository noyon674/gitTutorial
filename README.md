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
<p>7. Move working directory to staging area:<p/>

```
There are different ways

// for specific files -- with extension
1. git add file1 file2 file3 ...

// for all the file which are the same extension
2. git add *.extension

// all the file of the directory -- alson different extension fils
3. git add .
```