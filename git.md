# How to use git

### download

`$git clone [git repo]`

### upload

`$git init` (first recommend `git clone`)

`$git add *.`

`$git commit -m "[Message]" `

`$git push origin [branch]`

`$git remote #for check local repo` (usually origin)



<br><br>if you need sign in

```
$git config --global user.name "[My Name]" 
$git config --global user.email "[My Email]" 
```


<br><br>if you need check branch

```
$git branch #for check branch
$git branch [Branch Name] #for create branch
$git checkout [Branch Name] #for change branch
```


# .gitconfig

```
[user]
    name = MinkiJo
    email = ring9714@gmail.com
    username = MinkiJo
[core]
    editor = vim
[alias]
    # git add [file]
    a = add
    ap = add -p
    # git branch [branch name]
    b = branch
    ba = branch -a
    bd = branch -d
    bdd = branch -D
    br = branch -r
    cb = rev-parse --abbrev-ref HEAD  # current branch name.
    # git commit 
    cm = commit -m
    ca = commit --amend
    # git clone
    cl = clone
    clb = clone -b  # clone specific branch of repository.
    # git diff
    d = diff
    dh = diff HEAD 
    # git log
    lg = log --graph --abbrev-commit --decorate --all --oneline
    # git checkout 
    co = checkout
    cob = checkout -b
    # git push
    ps = push
    psf = push -f
    psu = push -u
    psom = push origin master
    psob = !git push origin $(git cb)
    # git pull
    pl = pull
    plob = !git pull origin $(git cb)
    # git remote
    r = remote
    rv = remote -v
    ra = remote add
    rao = remote add origin
    # git status
    s = status
    # git stash
    sa = stash apply
    sl = stash list
    sp = stash pop
    sd = stash drop

```


# .gitignore

```
# Compiled source #
###################
*.com
*.class
*.dll
*.exe
*.o
*.so

# Temporary files #
###################
*.swp
*.swo
*~

# Packages #
############
*.7z
*.dmg
*.gz
*.iso
*.jar
*.rar
*.tar
*.zip

# Logs #
########
*.log

# OS generated files #
######################
.DS_Store*
ehthumbs.db
Icon?
Thumbs.db

*.lock

# Byte-compiled / optimized / DLL files for python #
####################################################
__pycache__/
*.py[cod]
*$py.class
```
