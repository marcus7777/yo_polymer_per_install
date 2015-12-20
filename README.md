# yo_polymer_per_install
bash install as root
```
 sudo su
 apt-get install curl git -y
 cd
 wget https://nodejs.org/dist/v4.2.2/node-v4.2.2-linux-x64.tar.gz  --no-check-certificate
 # see https://nodejs.org/dist/v4.2.2/ for non linux-x64
 tar -xzf node-v*
 cd node-v*/
 cp bin/* /usr/bin
 cd
 wget https://npmjs.org/install.sh --no-check-certificate
 sh ./install.sh
 
 npm install generator-polymer gulp bower vulcanize firebase-tools yo -g 

 cd
 rm node* install.s* -rf
 
 exit

mkdir yo_polymer
cd yo_polymer
yo polymer
git init
git commit -am 'first commit'
