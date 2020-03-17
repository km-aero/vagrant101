# Vagrant and Virtual Box 101

Setup a simple ubunto machine

Allows us to manage virtual machines

## Basic Vagrant command
Vagrant:
- Init: creates vagrantfile
- Box: manages boxes on the machines
  - add
  - remove
  - list
  - update
- Up: creates a virtual machine
- ssh: log in to virtual machine (user vagrant pw vagrant)
- reload: shuts down and reloads machine


## Create ubunto 18.04 server
using Vagrants

## update packages using apt-get
sudo apt-get update -y

## Install packages using apt-get
sudo apt-get install nginx -y
- install package nginx

## Set up an internal IP
add the below into the vagrantfile:
- config.vm.network "private_network", ip: '<ip>'

## start a service using systemctl
sudo systemctl start nginx
- start the service nginx

## shows specific running services
ps aux | grep nginx
