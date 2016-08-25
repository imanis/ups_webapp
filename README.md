Front end project
===

Web client for UPS


Setup
===

 - clone the project
 - install dependency with
```
npm install
```
```
bower install
 ```
 - run a dev build
 ```
 grunt dev
```
 - copy the generated dist/ directory into apache server under a directory named webapp


### Endpoint configuration:

```sh
# Edit app/js/config.js and update
var ServerHost = "http://hostname:port"
# Don't forget to regenerate the dist/ folder after every modification !
```


### Osx steps for apache:

```sh
# Enable Apache on Mac OS X
apachectl start

# Create a new folder in apache
sudo mkdir /Library/WebServer/Documents/webapp/

# Copy dist/ to apache folder
sudo cp -R dist/*  /Library/WebServer/Documents/webapp/

# Go to http://localhost/webapp
```
