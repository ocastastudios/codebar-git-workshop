# Commands for the codebar git workshop

Copy and paste the following commands in the terminal to follow along with the slides

# Part 1

### The command line
_Slide 10:_


```

whoami
ls -al

```

### Configuration
_Slide 12:_


Configure git with your name and email.
Replace "Your name" and "name@example.com" in the commands below with your name and email address

```

git config --global user.name "Your name"
git config --global user.email "name@example.com"

```

### Git Init
_Slide 13:_


Make a new git repository

```
cd
```
on windows...
```
cd "My Documents"
```
on mac...
```
cd Documents
```

```
mkdir my-repo
cd my-repo
git init

```

_Slide 14:_


```
ls -al .git
```

### Our first commands
_Slide 15:_

Git status shows the current state of changes
Git log shows a list of commits

```
git status
git log
```

### Git add
_Slide 20:_


Create a file README.txt in the directory. Then add it to git
```
git add README.txt
git status
```

### Our first commit
_Slide 23:_

Commit our new file
```
git commit -m "My first commit"
git log
```

### Editing a file
_Slide 25:_

Make an edit to Readme.txt and then check the status
```
git status
git diff
```
### Git add and commit
_Slide 26:_

```
git add README.txt
git commit -m "Edited Readme"
```

### Checkout
_Slide 27:_

Discard changes using checkout.
Make some changes to README.txt and then...

```
git status
git checkout README.txt
git status
```

### Reset
_Slide 28:_

Remove a file tracked in git
```
touch hello.txt
git add hello.txt
git status
git reset hello.txt
git status
rm hello.txt
```

### Removing files
_Slide 29:_

Remove a file tracked in git
```
git rm README.txt
git status
git commit -m "Removed readme"
git log
```

### History
_Slide 30:_

```
git log
```

## Part 2

### Master
_Slide 36:_
```
git status
```

### Git branch
_Slide 37:_
```
git branch mybranch
git branch
```

### Checkout
_Slide 38:_
```
git checkout mybranch
touch mybranch.txt
git add mybranch.txt
git commit -m "commit on mybranch"
git log
```


### Parallel branches
_Slide 39:_
```
git checkout master
git log
```

### Vice versa
_Slide 40:_
```
touch master.txt
git add master.txt
git commit -m "commit on master"
git checkout mybranch
git log
```

### Git clone
_Slide 46:_

Clone the repository for this afternoon
```
cd ..
git clone https://github.com/ocastastudios/codebar-git-workshop.git
```