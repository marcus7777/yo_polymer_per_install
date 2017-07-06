# nodejs install
## bash install as root
```
  sudo su
```
## install, exit, Setup a polymer project
``` 
 curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
 apt-get install nodejs curl git -y
 npm install -g polymer-cli bower firebase-tools
 exit
 

mkdir polymer
cd polymer
polymer init
git init
git commit -am 'first commit'
```
