# yo_polymer_per_install
bash install as root
```
 sudo su
 cd
 wget https://iojs.org/dist/latest/iojs-v1.7.1-linux-x64.tar.gz
 tar xzf iojs-v1.7.1-linux-x64.tar.gz 
 cd iojs-v1.7.1-linux-x64/
 cp bin/* /usr/bin
 cd
 wget https://npmjs.org/install.sh
 chmod +x install.sh
 sudo ./install.sh
 npm install gulp -g 
 npm install bower -g
 npm install -g yo
 cd
 apt-get install ruby-full -y
 
 
 gem install compass
 ```
go to folder for app as normal user (not root)

```
npm install -g generator-polymer 
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

 
