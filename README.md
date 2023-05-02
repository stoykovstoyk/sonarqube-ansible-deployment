Sonarqube Server deployment script that you can use to deploy sonarqube on Vagrant VM and scan your project source code for vulnerabilities.

# Requirements #

* Vagrant 
* VirtualBox 

## How to use this repo on Ubuntu 22.04 ##

### Install Vagrant ###
```shell
$ sudo apt update -y
$ sudo apt install vagrant -y
```

### Install VirtualBox ###
``` shell
$ sudo apt install virtualbox -y
```

### Clone this repo & create Vagrant VM ###
```shell
$ git clone https://github.com/stoykovstoyk/sonarqube-ansible-deployment.git
$ cd sonarqube-ansible-deployment
$ vagrant up
```
### On your host machine add sonarqube.localhost to your hosts file ###
```shell
$ sudo sh -c 'echo "127.0.0.1 sonarqube.localhost" >> /etc/hosts'
```

### On your host machine navigate with your webbrowser to this URL ###
http://sonarqube.localhost:8080

### Default admin credentials are ###
user: admin

password: admin

You will be asked to change your password. Change it, then create new project and enjoy. 
