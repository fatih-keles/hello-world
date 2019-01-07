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