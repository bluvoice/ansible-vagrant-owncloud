# Owncloud Server 6.0.3
  
This repository contains a script that will automatically install Owncloud Server 6.0.3 onto VirtualBox VM using Ansible and Vagrant.

## Install prereqs

 * git
 * Ansible (tested with v1.4.1 on Ubuntu 13.04 and v1.4.5 on Ubuntu 12.04)
 * Vagrant (tested with v1.4.1 on Ubuntu 13.04 and on Ubuntu 12.04)
 * VirtualBox (tested with v4.2.10 on Ubuntu 13.04 and v4.2.18 on Ubuntu 12.04)

## Get the 64-bit Ubuntu 12.04 (precise) Vagrant box

$ vagrant box add precise64 http://files.vagrantup.com/precise64.box

## Grab this repository and run the installer

$ git clone http://github.com/bluvoice/ansible-vagrant-owncloud.git

$ cd ansible-vagrant-owncloud

$ ./install-owncloud

## OwnCloud web interface
The Web Interface is accessible at http://10.0.10.10/owncloud.
Administrator account: user=admin, password=adminp

## Vagrant-private-key permission
To solve ssh connection error, you can set the vagrant-private-key permission to none for group and others and repeat the installation. 




