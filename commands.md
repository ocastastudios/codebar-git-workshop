# Commands for the codebar git workshop

Copy and paste the following commands in the terminal to follow along with the slides

## Part 1

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
ls -al
ls -al .git
```

### Our first command
_Slide 15:_

Git status shows the current state of changes

```
git status
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
<!--
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
-->
### Removing files
_Slide 27:_

Remove a file tracked in git
```
git rm README.txt
git status
git commit -m "Removed readme"
```

### History
_Slide 28:_

Git log will give you a list of commits in reverse order.

If git log fits on more than one terminal screen it will go into a scrolling mode. press spacebar to scroll down a page, and when you get to the end press q to exit.

```
git log
```

## Part 2

### Master
_Slide 34:_
```
git status
```

### Git branch
_Slide 35:_
```
git branch mybranch
git branch
```

### Checkout
_Slide 36:_
```
git checkout mybranch
touch mybranch.txt
git add mybranch.txt
git commit -m "commit on mybranch"
git log
```


### Parallel branches
_Slide 37:_
```
git checkout master
git log
```

### Vice versa
_Slide 38:_
```
touch master.txt
git add master.txt
git commit -m "commit on master"
git checkout mybranch
git log
```

### Github
_Slide 43:_

The repo is at:

<https://repo.gitforthe.win>

or the full github url is

<https://github.com/ocastastudios/codebar-git-workshop>

### Git clone
_Slide 44:_

Clone the repository for this afternoon
```
cd ..
git clone https://github.com/ocastastudios/codebar-git-workshop.git
```

### Cloned repository

Let's look at the repository.

If git log fits on more than one terminal screen it will go into a scrolling mode. press spacebar to scroll down a page, and when you get to the end press q to exit.


_Slide 45:_
```
cd codebar-git-workshop
git status
git log
```

### Git fetch
_Slide 49:_
```
git fetch
git status
```

### Git pull
_Slide 50:_

```
git pull
```

### Pushing
_Slide 51:_

In the commands below, change **myname** to your actual name (for example _danielvanberzon_)
```
git branch myname
git checkout myname
```

### Make a commit
_Slide 52:_

Don't forget to change **myname** in the commands below to your name
```
touch myname.txt
git add myname.txt
git commit -m "branch commit"
```


### Git push
_Slide 53:_

Don't forget to change **myname** in the command below to your name
```
git push -u origin myname
```

### Pushed to github
_Slide 54:_

Don't forget to change **myname** in the command below to your name

```
git rm myname.txt
git commit -m "branch commit 2"
git push
```

### Git merge
_Slide 59:_

Go back into my-repo and list branches

```
cd ..
cd my-repo
git branch
```
## Part 3

### Git merge

_Slide 60:_

Merge mybranch into master
--no-edit means we don't have to create a merge commit message
```
git checkout master
git merge mybranch --no-edit.
```

### Merged branch

_Slide 61:_

If git log fits on more than one terminal screen it will go into a scrolling mode. press spacebar to scroll down a page, and when you get to the end press q to exit.

```
git log
```


## Afternoon:

### Useful git commands for the afternoon

Here is a list of useful git commands for when you are working on the afternoon exercise.

If the command has a word in angle brackets, e.g `<filename>` you should replace this with the appropriate name.

For example, if you want to add the file _README.txt_, the command `git add <filename>` should become `git add README.txt`

- View the current status

    ```
    git status
    ```

- View any un added changes
    
    ```
    git diff
    ```

- Add a file to the index

    ```
    git add <filename>
    ```

- Remove a file and add the deletion into the index

    ```
    git rm <filename>
    ```

- Make a commit

    ```
    git commit -m "<message>"
    ```

- See the commit history

    ```
    git log
    ```
    
    > If git log fits on more than one terminal screen it will go into a scrolling mode. press `spacebar` to scroll down a page, and when you get to the end press `q` to exit.

- List the branches

    ```
    git branch
    ```

- Create a branch

    ```
    git branch <branchname>
    ```

- Checkout onto a branch

    ```
    git checkout <branchname>
    ```

- Retrieve latest commit info from the remote repository

    ```
    git fetch
    ```

- Pull latest commits for a branch from the remote repository

    ```
    git pull
    ```

- Push a branch for the first time to the remote repository

    ```
    git push -u origin <branchname>
    ```

- Push a branch that's already been pushed once

    ```
    git push
    ```

- Lookup instructions on how to use a command

    ```
    git <command> --help
    ```

    > E.G `git checkout --help`
