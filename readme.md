## Quick Start 
### Check version
```git --version```
### Set user
```
git config --global user.name "Fatih Keles"
git config --global user.email "fatihkeles@gmail.com"
```
### check user
```
git config --global user.name
git config --global user.email
```

## Proxy 
Thanks to: https://gist.github.com/evantoli/f8c23a37eb3558ab8765
In the following form 
```git config --global http.proxy http://proxyuser:proxypwd@proxy.server.com:8080```

```
git config --global http.proxy http://www-proxy-lon.uk.oracle.com:80
git config --global https.proxy http://www-proxy-ams.nl.oracle.com:80
```
### unset 
```git config --global --unset http.proxy```
#### check 
```git config --global --get http.proxy```

## Create a local repository 
```
cd C:\GIT
mkdir hello-world
cd hello-world
git init
git status
```

### Add files
```
git add readme.md
git commit -m "Created readme"
```

### Check modifications
```git diff```

## Set Remote Repository
```
git config --global user.username "fatih-keles"
git config --global user.username
```

### Add remote connections
```git remote add <REMOTENAME> <URL>```
### Set a URL to a remote
```git remote set-url <REMOTENAME> <URL>```
### Pull in changes
```git pull <REMOTENAME> <BRANCHNAME>```
### View remote addresses
```git remote -v```
### Push changes
```git push <REMOTENAME> <BRANCH>```

### Set remote
```
git remote add origin https://github.com/fatih-keles/hello-world.git
git remote set-url origin https://github.com/fatih-keles/hello-world.git
```

### Push remote
```
git push origin master
```

### Clone remote
```git clone <URLFROMGITHUB>
git clone https://github.com/fatih-keles/patchwork.git
cd patchwork
git remote -v
```

http://fatih-keles.github.io/patchwork

### Also Connect to the Original Repository
You can name this remote connection anything you want, but typically people use the name 'upstream'
```
git remote add upstream https://github.com/jlord/patchwork.git
```

### create a branch 
```
git branch <BRANCHNAME>
git branch add-fatih-keles

git checkout <BRANCHNAME>
git checkout add-fatih-keles
git status 
```

### commit and push to remote
```git add CONTRIBUTORS/add-fatih-keles.txt
git commit -m "add fatih-keles"
git push origin add-fatih-keles```

### You can create and switch to a branch in one line
```git checkout -b <BRANCHNAME>```
### Create a new branch
```git branch <BRANCHNAME>```
### Move onto a branch
```git checkout <BRANCHNAME>```
### List the branches
```git branch```
### Rename a branch you're currently on
```git branch -m <NEWBRANCHNAME>```
### Verify what branch you're working on
```git status```

### See changes to the remote before you pull in
git fetch --dry-run

### GIT pull
```git pull origin add-fatih-keles```

### clean up
```
git checkout gh-pages
git merge add-fatih-keles
git branch -d add-fatih-keles
git push <REMOTENAME> --delete <BRANCHNAME>
git push origin --delete add-fatih-keles
git pull upstream gh-pages
```


### Merge a branch into current branch
```git merge <BRANCHNAME>```
### Change the branch you're working on
```git checkout <BRANCHNAME>```
### Delete a local branch
```git branch -d <BRANCHNAME>```
### Delete a remote branch
```git push <REMOTENAME> --delete <BRANCHNAME>```
### Pull from a remote branch
```git pull <REMOTENAME> <BRANCHNAME>```