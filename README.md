# yo_polymer_per_install
bash install as root
```
 sudo su
 cd
 wget https://iojs.org/dist/v2.3.0/iojs-v2.3.0-linux-x64.tar.xz
 tar xzf iojs-v2.3.0-linux-x64.tar.xz
 cd iojs-v*/
 cp bin/* /usr/bin
 cd
 wget https://npmjs.org/install.sh
 chmod +x install.sh
 apt-get install curl
 ./install.sh
 npm install gulp -g 
 npm install bower -g
 npm install -g yo
 cd
 rm iojs-v*-linux-x64* install.s*
 apt-get install ruby-full -y
 
 
 gem install compass
 npm install -g generator-polymer 
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

 
