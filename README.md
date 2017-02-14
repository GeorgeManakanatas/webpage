# HOME SHOWCASE
Basic webpage to showcase a home for rent and do basic booking and communication.

## Getting Started

### Prerequisites

The project is built using the MEAN stack on Centos7.
The frontend will use Vue and Bootstrap
The backend will use Node, Express, MongoDB and mongoose
```
Give examples
```
### Installing

#### Install MongoDB
Some of the following steps may require sudo privileges
The first step is to add MongoDB to the YUM repo
```
vim /etc/yum.repos.d/mongodb.repo
```
```
[mongodb]
name=MongoDB repo
baseurl=http://downloads-distro.mongodb.org/repo/redhat/os/x86_64/
gpgcheck=0
enabled=1
```
Then install the MongoDB packages
```
yum install mongodb-org
```
Enable the Mongodb Server
```
chkconfig  mongod  on
```
Start the Mongodb Server
```
service   mongod start
```
Check if the server is running
```
ps -ef  |  grep   mongo
```
Open a port on the firewall
```
firewall-cmd --zone=public --add-port=27017/tcp --permanent
```
```
firewall-cmd --reload
```
Now you should be able to access the database remotely
```
telnet 10.1.1.99  27017
```

#### Install Node.js from the EPEL Repository

Reconfigure access the repository by installing an available package.
```
sudo yum install epel-release
```
Install Node.js using regular yum commands.
```
sudo yum install nodejs
```
Check that the installation was successful
```
node --version
```

#### Install packages from npm

Go to the GDPR directory that houses the package.json file and install the
dependencies with npm.
```
sudo npm install
```


## Deployment

## Built With
* [Atom](https://atom.io/) - The text editor used
* [Postman](https://www.getpostman.com/) - For testing REST interaction with MongoDB
* [MongoDB](https://www.mongodb.com/) - As our main database
* [Mongoose](http://mongoosejs.com/) - Object modeling for Node.js
* [Node.js](https://nodejs.org/en/) - A JavaScript runtime built on Chrome's V8 engine.
* [Express.js](http://expressjs.com/) - A web framework for Node.js
* [Nodemailer](https://nodemailer.com/) - Node.js integrated emailer
* [Angular.js](https://angularjs.org/) - Front-end web application framework
* [Bootstrap](http://getbootstrap.com/) - Front-end framework
* [Bower](https://bower.io/) - Package manager

## Author
George  Manakanatas

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments
