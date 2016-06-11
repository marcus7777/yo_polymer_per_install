# yo_polymer_per_install
bash install as root
```
 sudo su
 apt-get install curl git -y
 cd
 wget https://nodejs.org/dist/v6.2.1/node-v6.2.1-linux-x64.tar.xz  --no-check-certificate
 # see https://nodejs.org/ for non linux-x64
 tar -xf node-v*
 cd node-v*/
 cp bin/* /usr/bin
 cd
 wget https://npmjs.org/install.sh --no-check-certificate
 sh ./install.sh
 
 npm install -g polymer-cli bower

 cd
 rm node* install.s* -rf
 
 exit

mkdir yo_polymer
cd yo_polymer
yo polymer
git init
git commit -am 'first commit'
