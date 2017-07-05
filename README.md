# yo_polymer_per_install
bash install as root
```
 sudo su
 apt-get install curl git -y
 cd
 curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
 
 cd
 wget https://npmjs.org/install.sh --no-check-certificate
 sh ./install.sh
 
 npm install -g polymer-cli bower firebase-tools

 cd
 rm node-v* install.s* -rf
 
 exit

mkdir polymer
cd polymer
polymer init
git init
git commit -am 'first commit'
