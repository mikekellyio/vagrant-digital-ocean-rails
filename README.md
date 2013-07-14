# Get up and running

## 1. Install Vagrant
https://www.vagrantup.org/

## 2. Install berkshelf
``
  $ vagrant plugin install vagrant-berkshelf
  Installing the 'vagrant-berkshelf' plugin. This can take a few minutes...
  Installed the plugin 'vagrant-berkshelf (1.2.0)!'
  $ bundle
``

## 3. Install Digital Ocean Provider

Installation of the provider requires two steps:

1. Install the provider plugin using the Vagrant command-line interface:
``
  $ vagrant plugin install vagrant-digitalocean
``
2. Install the default provider box:
``
  $ vagrant box add digital_ocean https://github.com/smdahlen/vagrant-digitalocean/raw/master/box/digital_ocean.box
``

## 4. Install chef cookbooks
``
  $ berks install
``

## 5. Build the VM
``
  $ vagrant up
``

# Usage

To login to the VM run:

``
  $ vagrant ssh
``

When you are done, exit the VM and run the following command to suspend it until later.

``
  $ vagrant suspend
``

Resume work at anytime:

``
  $ vagrant up
``
