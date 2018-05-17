# Commands for the codebar git workshop

Copy and paste the following commands in the terminal to follow along with the slides

## The command line
_Slide 10:_

```

whoami
ls -al

```

## Configuration
_Slide 12:_

Configure git with your name and email.
Replace "Your name" and "name@example.com" in the commands below with your name and email address

```

git config --global user.name "Your name"
git config --global user.email "name@example.com"

```

## Git Init
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

## Our first commands
_Slide 15:_
Git status shows the current state of changes
Git log shows a list of commits

```
git status
git log
```

## Git add
_Slide 20:_

Create a file Readme.txt in the directory. Then add it to git
```
git add README.txt
git status
```

## Our first commit
_Slide 23:_
Commit our new file
```
git commit -m "My first commit"
git log

```