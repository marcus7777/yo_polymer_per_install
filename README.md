# yo_polymer_per_install
bash install as root
```
 sudo su
 apt-get install curl git -y
 cd
 wget https://nodejs.org/dist/v6.11.0/node-v6.11.0-linux-x64.tar.xz  --no-check-certificate
 # see https://nodejs.org/ for non linux-x64
 tar -xf node-v*
 cd node-v*/
 cp bin/* /usr/bin
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
