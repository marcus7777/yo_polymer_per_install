# yo_polymer_per_install
bash install as root
```
 sudo su
 apt-get install git -y
 cd
 wget https://nodejs.org/dist/v4.2.2/node-v4.2.2-linux-x64.tar.gz  --no-check-certificate
 # see https://nodejs.org/dist/v4.2.2/ for non linux-x64
 tar -xzf node-v*
 cd node-v*/
 cp bin/* /usr/bin
 cd
 wget https://npmjs.org/install.sh --no-check-certificate
 chmod +x install.sh
 apt-get install curl -y
 ./install.sh
 npm install generator-polymer gulp bower vulcanize firebase-tools yo -g 

 cd
 rm iojs-v*-linux-x64* install.s* -r
 
 exit

yo polymer
git init
sudo crontab -e
```
add
```
@reboot sudo su -c "cd /home/marcus7777_gmail_com/;gulp serve"
* * * * * cd /home/marcus7777_gmail_com/ && git pull
```
if you need it serving on port 80 add update gulpfile.js:

```
...
// Watch Files For Changes & Reload
gulp.task('serve', ['styles', 'elements'], function () {
  browserSync({
    notify: false,
    port: 80,
    ...
```

 
